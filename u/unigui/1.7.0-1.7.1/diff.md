# Comparing `tmp/unigui-1.7.0.tar.gz` & `tmp/unigui-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.7.0.tar", last modified: Sun Jul  2 15:39:08 2023, max compression
+gzip compressed data, was "dist/unigui-1.7.1.tar", last modified: Mon Jul  3 18:29:36 2023, max compression
```

## Comparing `unigui-1.7.0.tar` & `unigui-1.7.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    11822 2023-07-02 15:37:04.000000 unigui-1.7.0/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.7.0/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.7.0/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.7.0/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2396 2023-07-02 15:25:42.000000 unigui-1.7.0/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/css/274.13cee13e.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    44049 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/js/274.9d2f3775.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/js/app.59c7eb11.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-02 15:31:50.000000 unigui-1.7.0/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.7.0/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-02 15:38:35.000000 unigui-1.7.0/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18977 2023-07-02 15:39:08.000000 unigui-1.7.0/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-02 15:39:08.000000 unigui-1.7.0/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18672 2023-07-02 15:37:14.000000 unigui-1.7.0/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.7.0/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18977 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.7.0/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-02 15:39:08.000000 unigui-1.7.0/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    11822 2023-07-02 15:37:04.000000 unigui-1.7.1/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.7.1/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.7.1/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.7.1/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2396 2023-07-02 15:25:42.000000 unigui-1.7.1/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/css/vendor.49a52e8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/css/572.13cee13e.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/js/app.feb97290.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    44787 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/js/572.4a65c656.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-03 18:22:24.000000 unigui-1.7.1/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.7.1/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-03 18:29:08.000000 unigui-1.7.1/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19119 2023-07-03 18:29:36.000000 unigui-1.7.1/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-03 18:29:36.000000 unigui-1.7.1/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18814 2023-07-03 18:26:00.000000 unigui-1.7.1/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.7.1/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19119 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.7.1/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-03 18:29:36.000000 unigui-1.7.1/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.7.0/unigui/manager.py` & `unigui-1.7.1/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/guielements.py` & `unigui-1.7.1/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/server.py` & `unigui-1.7.1/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/utils.py` & `unigui-1.7.1/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/favicon.ico` & `unigui-1.7.1/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/css/274.13cee13e.css` & `unigui-1.7.1/unigui/web/css/572.13cee13e.css`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.7.1/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/icons/favicon-96x96.png` & `unigui-1.7.1/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/icons/favicon-16x16.png` & `unigui-1.7.1/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/icons/favicon-32x32.png` & `unigui-1.7.1/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/icons/favicon-128x128.png` & `unigui-1.7.1/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.7.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.7.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.7.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.7.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.7.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/js/430.591e9a73.js` & `unigui-1.7.1/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/js/274.9d2f3775.js` & `unigui-1.7.1/unigui/web/js/572.4a65c656.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,134 +1,134 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [274], {
-        9274: (e, t, a) => {
+    [572], {
+        5572: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Jt
             });
-            var l = a(3673),
-                s = a(2323);
-            const i = (0, l._)("div", {
+            var s = a(3673),
+                l = a(2323);
+            const i = (0, s._)("div", {
                     class: "q-pa-lg"
                 }, null, -1),
-                o = (0, l._)("div", {
+                o = (0, s._)("div", {
                     class: "q-pa-lg"
                 }, null, -1);
 
             function n(e, t, a, n, d, r) {
-                const c = (0, l.up)("q-item-label"),
-                    h = (0, l.up)("element"),
-                    u = (0, l.up)("q-tab"),
-                    p = (0, l.up)("q-tabs"),
-                    g = (0, l.up)("q-toolbar"),
-                    m = (0, l.up)("q-header"),
-                    f = (0, l.up)("zone"),
-                    w = (0, l.up)("q-page"),
-                    y = (0, l.up)("q-page-container"),
-                    b = (0, l.up)("q-layout");
-                return (0, l.wg)(), (0, l.j4)(b, {
+                const c = (0, s.up)("q-item-label"),
+                    h = (0, s.up)("element"),
+                    u = (0, s.up)("q-tab"),
+                    p = (0, s.up)("q-tabs"),
+                    g = (0, s.up)("q-toolbar"),
+                    m = (0, s.up)("q-header"),
+                    f = (0, s.up)("zone"),
+                    y = (0, s.up)("q-page"),
+                    w = (0, s.up)("q-page-container"),
+                    b = (0, s.up)("q-layout");
+                return (0, s.wg)(), (0, s.j4)(b, {
                     view: "lHh Lpr lFf"
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(m, {
+                    default: (0, s.w5)((() => [(0, s.Wm)(m, {
                         elevated: ""
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(g, null, {
-                            default: (0, l.w5)((() => [(0, l.Wm)(c, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(g, null, {
+                            default: (0, s.w5)((() => [(0, s.Wm)(c, {
                                 class: "text-h5"
                             }, {
-                                default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.screen.header ? e.screen.header : ""), 1)])),
+                                default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
-                            }), i, ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.screen.toolbar, (t => ((0, l.wg)(), (0, l.j4)(h, {
+                            }), i, ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.screen.toolbar, (t => ((0, s.wg)(), (0, s.j4)(h, {
                                 class: "q-ma-xs bg-blue-5",
                                 data: t,
                                 pdata: e.data
-                            }, null, 8, ["data", "pdata"])))), 256)), o, (0, l.Wm)(p, {
+                            }, null, 8, ["data", "pdata"])))), 256)), o, (0, s.Wm)(p, {
                                 class: "text-teal",
                                 align: "center",
                                 "inline-label": "",
                                 dense: "",
                                 modelValue: e.tab,
                                 "onUpdate:modelValue": t[0] || (t[0] = t => e.tab = t),
                                 style: {
                                     float: "center"
                                 }
                             }, {
-                                default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.menu, (t => ((0, l.wg)(), (0, l.iD)("div", null, [t.icon ? ((0, l.wg)(), (0, l.j4)(u, {
+                                default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.menu, (t => ((0, s.wg)(), (0, s.iD)("div", null, [t.icon ? ((0, s.wg)(), (0, s.j4)(u, {
                                     key: 0,
                                     class: "justify-center text-white shadow-2",
                                     name: t.name,
                                     icon: t.icon,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
-                                }, null, 8, ["name", "icon", "label", "onClick"])) : (0, l.kq)("", !0), t.icon ? (0, l.kq)("", !0) : ((0, l.wg)(), (0, l.j4)(u, {
+                                }, null, 8, ["name", "icon", "label", "onClick"])) : (0, s.kq)("", !0), t.icon ? (0, s.kq)("", !0) : ((0, s.wg)(), (0, s.j4)(u, {
                                     key: 1,
                                     class: "justify-center text-white shadow-2",
                                     name: t.name,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
                             }, 8, ["modelValue"])])),
                             _: 1
                         })])),
                         _: 1
-                    }), (0, l.Wm)(y, null, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(w, {
+                    }), (0, s.Wm)(w, null, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(y, {
                             class: "flex justify-center centers"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Wm)(f, {
+                            default: (0, s.w5)((() => [(0, s.Wm)(f, {
                                 data: e.screen.blocks
                             }, null, 8, ["data"])])),
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 })
             }
             a(71);
 
             function d(e, t, a, i, o, n) {
-                const d = (0, l.up)("q-icon"),
-                    r = (0, l.up)("q-item-section"),
-                    c = (0, l.up)("q-item-label"),
-                    h = (0, l.up)("q-item");
-                return (0, l.wg)(), (0, l.j4)(h, {
+                const d = (0, s.up)("q-icon"),
+                    r = (0, s.up)("q-item-section"),
+                    c = (0, s.up)("q-item-label"),
+                    h = (0, s.up)("q-item");
+                return (0, s.wg)(), (0, s.j4)(h, {
                     clickable: "",
                     tag: "a",
                     target: "_blank",
                     onClick: e.send
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                    default: (0, s.w5)((() => [(0, s.Wm)(r, {
                         avatar: ""
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(d, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(d, {
                             name: e.icon
                         }, null, 8, ["name"])])),
                         _: 1
-                    }), (0, l.Wm)(r, null, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(c, null, {
-                            default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.name), 1)])),
+                    }), (0, s.Wm)(r, null, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(c, null, {
+                            default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.name), 1)])),
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 }, 8, ["onClick"])
             }
             var r, c = a(698),
                 h = a(8603);
             let u = null,
                 p = {},
                 g = !0;
             const m = 136,
                 f = 400,
-                w = `height: ${m}px; width: ${f}px`;
+                y = `height: ${m}px; width: ${f}px`;
 
-            function y(e) {
+            function w(e) {
                 let t = e.minheight ? e.minheight : m,
                     a = e.minwidth ? e.minwidth : f;
                 return `height: ${t}px; width: ${a}px`
             }
             let b = {},
                 k = {};
             const v = ["error", "progress", "warning", "info"];
@@ -146,18 +146,18 @@
             }
             let j, S = 0;
 
             function z() {
                 for (let [e, t] of Object.entries(k)) t.styleSize = null
             }
 
-            function A(e, t, a, l = "?") {
-                let s = ++S,
-                    i = [e.pdata.name, e.data.name, l, t, s];
-                q(i), p[s] = a
+            function A(e, t, a, s = "?") {
+                let l = ++S,
+                    i = [e.pdata.name, e.data.name, s, t, l];
+                q(i), p[l] = a
             }
 
             function Z() {
                 b = {}, k = {}
             }
 
             function M(e, t) {
@@ -165,62 +165,62 @@
             }
 
             function D(e) {
                 if (e.multi)
                     for (let [t, a] of e.update.entries())
                         if (a.length > 1) {
                             a.reverse();
-                            let l = a.join("@"),
-                                s = k[l];
-                            M(s, e.data[t])
+                            let s = a.join("@"),
+                                l = k[s];
+                            M(l, e.data[t])
                         } else {
-                            let l = b[a[0]];
-                            Object.assign(l.data, e.data[t])
+                            let s = b[a[0]];
+                            Object.assign(s.data, e.data[t])
                         }
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
                         t = k[e]
                     } else t = b[a[0]];
-                    M(t, e.data), 1 == a.length && (0, h.delay)(W, 200, t)
+                    M(t, e.data), 1 == a.length && (0, h.delay)(E, 200, t)
                 }
             }
 
             function $(e) {
                 typeof e.answer == String ? u.showError() : p[e.id](e.answer), delete p[e.id]
             }
 
             function V(e) {
                 let t = [];
-                for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
+                for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function O() {
-                for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = y(t.data));
-                (0, l.Y3)((() => {
+            function K() {
+                for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = w(t.data));
+                (0, s.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            W()
+                            E()
                         }))
                     }))
                 }))
             }
-            let Q = _.debounce(O, 200);
+            let O = _.debounce(K, 200);
 
-            function W(e) {
+            function E(e) {
                 Array.isArray(e) && (e = null), j && (j.disconnect(), j = null), g && console.log("------------------recalc design");
-                const t = H(e),
-                    a = E(e);
-                for (let [l, s] of Object.entries(t)) {
-                    let e = k[l];
-                    const [t, i] = a[l];
+                const t = Q(e),
+                    a = W(e);
+                for (let [s, l] of Object.entries(t)) {
+                    let e = k[s];
+                    const [t, i] = a[s];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = b[d];
                     for (let a of r.data.childs)
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
@@ -230,25 +230,25 @@
                             }
                         } else if (a.name == e.data.name) {
                         o = e;
                         break
                     }
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
-                    let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
-                    e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
+                    let h = s.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
+                    e.styleSize = `height: ${h+l}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function H(e) {
+            function Q(e) {
                 const t = u.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
-                let l = {},
-                    s = new Map,
+                let s = {},
+                    l = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
                         n = t ? V(d) : [
@@ -256,127 +256,127 @@
                         ];
                     for (let a of n) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
                         o.push([e, a])
                     }
                     o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
-                    for (let l of o) {
-                        let t = l[1];
+                    for (let s of o) {
+                        let t = s[1];
                         (0, c.hu)(Array.isArray(t));
                         const i = [];
                         for (let [e, a] of Object.entries(k))
                             if (a.expanding_height) {
-                                let [l, o] = e.split("@");
+                                let [s, o] = e.split("@");
                                 if (t.find((e => e.name == o))) {
                                     let e = !0;
                                     const t = a.geom();
-                                    for (let [l, o] of i.entries()) {
+                                    for (let [s, o] of i.entries()) {
                                         let n = o.geom();
                                         if (o !== a && n.top == t.top) {
-                                            n.scrollHeight < t.scrollHeight && (i[l] = a), e = !1, s.set(a.fullname, o.fullname);
+                                            n.scrollHeight < t.scrollHeight && (i[s] = a), e = !1, l.set(a.fullname, o.fullname);
                                             break
                                         }
                                     }
                                     e && i.push(a)
                                 }
-                            } i.length && e.push([a - l[0] - 64, i])
+                            } i.length && e.push([a - s[0] - 64, i])
                     }
-                    for (let [a, s] of e) {
-                        s.sort(((e, t) => e.geom().scrollHeight < t.geom().scrollHeight));
-                        let e = s.length;
-                        for (let i of s) i.fullname in l && (e--, a -= l[i.fullname]);
+                    for (let [a, l] of e) {
+                        l.sort(((e, t) => e.geom().scrollHeight < t.geom().scrollHeight));
+                        let e = l.length;
+                        for (let i of l) i.fullname in s && (e--, a -= s[i.fullname]);
                         let t = 0;
-                        for (let i of s)
-                            if (!(i.fullname in l)) {
-                                let s, o = a / e;
-                                if (1 == e) s = o;
-                                else if (s = Math.floor(o), o - s) {
-                                    t += o - s;
+                        for (let i of l)
+                            if (!(i.fullname in s)) {
+                                let l, o = a / e;
+                                if (1 == e) l = o;
+                                else if (l = Math.floor(o), o - l) {
+                                    t += o - l;
                                     let e = Math.round(t) - t;
-                                    e < .001 && e > -.001 && (s += Math.round(t), t = 0)
+                                    e < .001 && e > -.001 && (l += Math.round(t), t = 0)
                                 }
-                                "docviewer" == i.type ? l[i.fullname] = s + 4 : l[i.fullname] = s
+                                "docviewer" == i.type ? s[i.fullname] = l + 4 : s[i.fullname] = l
                             }
                     }
                 }
-                let n = Array.from(s.entries());
-                n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
-                for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
-                return l
+                let n = Array.from(l.entries());
+                n.sort(((e, t) => e[0] in s || e[1] in s ? -1 : 1));
+                for (let [d, r] of n) r in s ? s[d] = s[r] : s[r] = s[d];
+                return s
             }
 
-            function E(e) {
+            function W(e) {
                 e = null;
                 const t = e ? [e] : u.screen.blocks;
                 let a = window.innerWidth - 30,
-                    l = [],
-                    s = {};
+                    s = [],
+                    l = {};
                 for (let n of t)
-                    if (0 == l.length)
+                    if (0 == s.length)
                         if (Array.isArray(n))
-                            for (let e of n) l.push(Array.isArray(e) ? e : [e]);
-                        else l = [
+                            for (let e of n) s.push(Array.isArray(e) ? e : [e]);
+                        else s = [
                             [n]
                         ];
                 else {
                     let e = [];
                     if (Array.isArray(n))
                         for (let t of n)
-                            for (let a of l) e.push(Array.isArray(t) ? a.concat(t) : [...a, t]);
+                            for (let a of s) e.push(Array.isArray(t) ? a.concat(t) : [...a, t]);
                     else
-                        for (let t of l) e.push([...t, n]);
-                    l = e
+                        for (let t of s) e.push([...t, n]);
+                    s = e
                 }
-                l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
+                s.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
                 const i = [];
                 let o = new Map;
-                for (let n of l) {
+                for (let n of s) {
                     let e = Array.isArray(n) ? n[n.length - 1] : n,
                         t = b[e.name].$el.getBoundingClientRect().right;
                     e = Array.isArray(n) ? n[0] : n;
-                    let l = b[e.name].$el.getBoundingClientRect().left,
-                        s = a - t + l - 10;
+                    let s = b[e.name].$el.getBoundingClientRect().left,
+                        l = a - t + s - 10;
                     const d = [];
                     for (let [a, i] of Object.entries(k))
                         if (i.expanding_width) {
                             let e = a.split("@")[1];
                             if (n.find((t => t.name == e))) {
                                 let e = !0,
                                     t = i.geom().left;
-                                for (let [a, l] of d.entries())
-                                    if (l !== i && l.geom().left == t) {
-                                        l.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, o.set(l.fullname, i.fullname)) : o.set(i.fullname, l.fullname), e = !1;
+                                for (let [a, s] of d.entries())
+                                    if (s !== i && s.geom().left == t) {
+                                        s.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, o.set(s.fullname, i.fullname)) : o.set(i.fullname, s.fullname), e = !1;
                                         break
                                     } e && d.push(i)
                             }
-                        } d.length && i.push([s, d])
+                        } d.length && i.push([l, d])
                 }
                 for (let [n, d] of i) {
                     d.sort(((e, t) => e.geom().scrollWidth - t.geom().scrollWidth));
                     let e = d.length,
                         t = {};
                     for (let a of d) {
-                        let l = s[a.fullname];
-                        l && (e--, n -= l[0] / l[1]);
+                        let s = l[a.fullname];
+                        s && (e--, n -= s[0] / s[1]);
                         let i = a.pdata ? a.pdata.name : a.name;
                         t[i] ? t[i]++ : t[i] = 1
                     }
                     for (let a of d) {
-                        let l = s[a.fullname];
-                        if (void 0 === l) {
-                            let l = a.pdata ? a.pdata.name : a.name;
-                            s[a.fullname] = [Math.floor(n / e), t[l]]
+                        let s = l[a.fullname];
+                        if (void 0 === s) {
+                            let s = a.pdata ? a.pdata.name : a.name;
+                            l[a.fullname] = [Math.floor(n / e), t[s]]
                         }
                     }
                 }
-                for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
-                return s
+                for (let [n, d] of o.entries()) d in l ? l[n] = l[d] : l[d] = l[n];
+                return l
             }
-            const U = (0, l.aZ)({
+            const H = (0, s.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
                         q(["root", this.name])
                     }
                 },
                 props: {
@@ -386,28 +386,28 @@
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var N = a(4260),
-                F = a(3414),
-                K = a(2035),
+            var U = a(4260),
+                N = a(3414),
+                F = a(2035),
                 P = a(4554),
                 T = a(2350),
                 I = a(7518),
                 R = a.n(I);
-            const B = (0, N.Z)(U, [
+            const L = (0, U.Z)(H, [
                     ["render", d]
                 ]),
-                L = B;
-            R()(U, "components", {
-                QItem: F.Z,
-                QItemSection: K.Z,
+                B = L;
+            R()(H, "components", {
+                QItem: N.Z,
+                QItemSection: F.Z,
                 QIcon: P.Z,
                 QItemLabel: T.Z
             });
             const Y = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
@@ -415,23 +415,23 @@
                     class: "q-col-gutter-sm"
                 },
                 G = {
                     key: 0,
                     class: "column q-col-gutter-sm"
                 };
 
-            function J(e, t, a, s, i, o) {
-                const n = (0, l.up)("zone", !0),
-                    d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", X, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", G, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+            function J(e, t, a, l, i, o) {
+                const n = (0, s.up)("zone", !0),
+                    d = (0, s.up)("block");
+                return e.data instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", Y, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data, (e => ((0, s.wg)(), (0, s.iD)("div", X, [e instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", G, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e, (e => ((0, s.wg)(), (0, s.j4)(n, {
                     data: e
-                }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
+                }, null, 8, ["data"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e
-                }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
+                }, null, 8, ["data"]))])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
             const ee = {
                     class: "row"
                 },
@@ -439,86 +439,86 @@
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
                     }
                 },
                 ae = ["data", "pdata"],
-                le = {
+                se = {
                     key: 0,
                     class: "row"
                 },
-                se = ["data", "pdata"],
+                le = ["data", "pdata"],
                 ie = {
                     key: 0,
                     class: "row"
                 };
 
             function oe(e, t, a, i, o, n) {
-                const d = (0, l.up)("element"),
-                    r = (0, l.up)("q-icon"),
-                    c = (0, l.up)("q-scroll-area"),
-                    h = (0, l.up)("q-card");
-                return (0, l.wg)(), (0, l.j4)(h, {
+                const d = (0, s.up)("element"),
+                    r = (0, s.up)("q-icon"),
+                    c = (0, s.up)("q-scroll-area"),
+                    h = (0, s.up)("q-card");
+                return (0, s.wg)(), (0, s.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", ee, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, s.w5)((() => [(0, s._)("div", ee, [e.data.logo ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
+                    }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, s.wg)(), (0, s.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", te, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.top_childs, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, s.kq)("", !0), "_" != e.name[0] ? ((0, s.wg)(), (0, s.iD)("p", te, (0, l.zw)(e.name), 1)) : (0, s.kq)("", !0), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data.top_childs, (t => ((0, s.wg)(), (0, s.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
+                    }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, s.wg)(), (0, s.j4)(c, {
                         key: 0,
-                        style: (0, s.j5)(e.styleSize),
+                        style: (0, l.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
-                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
+                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data.childs, (t => ((0, s.wg)(), (0, s.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                        }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", se, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
+                        }, null, 8, ["data", "pdata"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
                         _: 1
-                    }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
+                    }, 8, ["style", "thumb-style", "bar-style"])) : ((0, s.wg)(!0), (0, s.iD)(s.HY, {
                         key: 1
-                    }, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
+                    }, (0, s.Ko)(e.data.childs, (t => ((0, s.wg)(), (0, s.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ie, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ie, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["data", "pdata"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                     _: 1
                 })
             }
             var ne = a(8880);
-            const de = e => ((0, l.dD)("data-v-606d07c3"), e = e(), (0, l.Cn)(), e),
+            const de = e => ((0, s.dD)("data-v-606d07c3"), e = e(), (0, s.Cn)(), e),
                 re = ["width", "height"],
                 ce = ["src"],
                 he = {
                     key: 16,
                     class: "web-camera-container"
                 },
                 ue = {
@@ -529,151 +529,151 @@
                 },
                 ge = {
                     key: 1
                 },
                 me = {
                     class: "camera-loading"
                 },
-                fe = de((() => (0, l._)("ul", {
+                fe = de((() => (0, s._)("ul", {
                     class: "loader-circle"
-                }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                we = [fe],
-                ye = ["height"],
+                }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
+                ye = [fe],
+                we = ["height"],
                 be = ["height"],
                 ke = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ve = de((() => (0, l._)("img", {
+                ve = de((() => (0, s._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
                 xe = [ve],
                 Ce = {
                     key: 2,
                     class: "camera-download"
                 };
 
             function qe(e, t, a, i, o, n) {
-                const d = (0, l.up)("q-icon"),
-                    r = (0, l.up)("q-img"),
-                    c = (0, l.up)("q-badge"),
-                    h = (0, l.up)("q-select"),
-                    u = (0, l.up)("q-checkbox"),
-                    p = (0, l.up)("q-toggle"),
-                    g = (0, l.up)("q-btn-toggle"),
-                    m = (0, l.up)("utable"),
-                    f = (0, l.up)("linechart"),
-                    w = (0, l.up)("q-input"),
-                    y = (0, l.up)("q-tree"),
-                    b = (0, l.up)("q-scroll-area"),
-                    k = (0, l.up)("q-separator"),
-                    v = (0, l.up)("q-uploader"),
-                    x = (0, l.up)("cgraph"),
-                    C = (0, l.up)("q-btn"),
-                    q = (0, l.up)("q-tooltip");
-                return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
+                const d = (0, s.up)("q-icon"),
+                    r = (0, s.up)("q-img"),
+                    c = (0, s.up)("q-badge"),
+                    h = (0, s.up)("q-select"),
+                    u = (0, s.up)("q-checkbox"),
+                    p = (0, s.up)("q-toggle"),
+                    g = (0, s.up)("q-btn-toggle"),
+                    m = (0, s.up)("utable"),
+                    f = (0, s.up)("linechart"),
+                    y = (0, s.up)("q-input"),
+                    w = (0, s.up)("q-tree"),
+                    b = (0, s.up)("q-scroll-area"),
+                    k = (0, s.up)("q-separator"),
+                    v = (0, s.up)("q-uploader"),
+                    x = (0, s.up)("cgraph"),
+                    C = (0, s.up)("q-btn"),
+                    q = (0, s.up)("q-tooltip");
+                return "image" == e.type ? ((0, s.wg)(), (0, s.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
                     onClick: (0, ne.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
-                    style: (0, s.j5)(e.elemSize)
+                    style: (0, l.j5)(e.elemSize)
                 }, {
-                    default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
+                    default: (0, s.w5)((() => [e.data.header ? ((0, s.wg)(), (0, s.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
                         onClick: t[0] || (t[0] = (0, ne.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
-                    }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
+                    }, (0, l.zw)(e.data.header), 1)) : (0, s.kq)("", !0), e.value ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "gray",
                         style: {
                             "font-size": "2em",
                             top: "8px",
                             left: "8px"
                         }
-                    })) : (0, l.kq)("", !0)])),
+                    })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["src", "onClick", "style"])) : "select" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
+                }, 8, ["src", "onClick", "style"])) : "select" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
                     key: 1,
                     "transition-show": "flip-up",
                     "transition-hide": "flip-down",
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[1] || (t[1] = t => e.value = t),
                     options: e.data.options
-                }, (0, l.Nv)({
+                }, (0, s.Nv)({
                     _: 2
                 }, [e.showname ? {
                     name: "prepend",
-                    fn: (0, l.w5)((() => [(0, l.Wm)(c, {
+                    fn: (0, s.w5)((() => [(0, s.Wm)(c, {
                         color: "secondary"
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.name), 1)])),
+                        default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.name), 1)])),
                         _: 1
                     })])),
                     key: "0"
-                } : void 0]), 1032, ["modelValue", "options"])) : "check" == e.type ? ((0, l.wg)(), (0, l.j4)(u, {
+                } : void 0]), 1032, ["modelValue", "options"])) : "check" == e.type ? ((0, s.wg)(), (0, s.j4)(u, {
                     key: 2,
                     "left-label": "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[2] || (t[2] = t => e.value = t),
                     label: e.nameLabel,
                     "checked-icon": "task_alt",
                     "unchecked-icon": "highlight_off"
-                }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, l.wg)(), (0, l.j4)(p, {
+                }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.j4)(g, {
                     key: 4,
                     push: "",
                     "no-caps": "",
                     width: "400px",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
                 }, {
-                    default: (0, l.w5)((() => [e.showname ? ((0, l.wg)(), (0, l.j4)(c, {
+                    default: (0, s.w5)((() => [e.showname ? ((0, s.wg)(), (0, s.j4)(c, {
                         key: 0,
                         color: "secondary"
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.name), 1)])),
+                        default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.name), 1)])),
                         _: 1
-                    })) : (0, l.kq)("", !0)])),
+                    })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["modelValue", "options"])) : "table" == e.type ? ((0, l.wg)(), (0, l.j4)(m, {
+                }, 8, ["modelValue", "options"])) : "table" == e.type ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 5,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, s.wg)(), (0, s.j4)(f, {
                     key: 6,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, s.wg)(), (0, s.j4)(y, {
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
-                }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
+                }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
                     key: 8,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     "use-input": "",
                     "hide-selected": "",
                     borderless: "",
@@ -681,352 +681,352 @@
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
                     onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
-                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
+                }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, s.wg)(), (0, s.j4)(b, {
                     key: 9,
-                    style: (0, s.j5)(e.styleSize),
+                    style: (0, l.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(y, {
+                    default: (0, s.w5)((() => [(0, s.Wm)(w, {
                         nodes: e.treeNodes,
                         selected: e.value,
                         "onUpdate:selected": t[7] || (t[7] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[8] || (t[8] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": "",
                         "selected-color": "blue-10"
                     }, null, 8, ["nodes", "selected", "expanded"])])),
                     _: 1
-                }, 8, ["style", "thumb-style", "bar-style"])) : "docviewer" == e.type ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("textarea", {
+                }, 8, ["style", "thumb-style", "bar-style"])) : "docviewer" == e.type ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("textarea", {
                     key: 10,
                     class: "textarea",
                     "onUpdate:modelValue": t[9] || (t[9] = t => e.value = t),
                     filled: "",
                     type: "textarea",
-                    style: (0, s.j5)(e.elemSize)
+                    style: (0, l.j5)(e.elemSize)
                 }, null, 4)), [
                     [ne.nr, e.value]
-                ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
+                ]) : "line" == e.type ? ((0, s.wg)(), (0, s.j4)(k, {
                     key: 11,
                     color: "green"
-                })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
+                })) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
-                }, [(0, l._)("source", {
+                }, [(0, s._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, ce)], 8, re)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                }, null, 8, ce)], 8, re)) : "gallery" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 13,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
-                    style: (0, s.j5)(e.elemSize),
+                    style: (0, l.j5)(e.elemSize),
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
                     key: 15,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", he, [(0, l._)("div", ue, [(0, l._)("button", {
-                    class: (0, s.C_)(["button is-rounded", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", he, [(0, s._)("div", ue, [(0, s._)("button", {
+                    class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[10] || (t[10] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", ge, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", pe, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", me, we, 512), [
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", ge, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", me, ye, 512), [
                     [ne.F8, e.isCameraOpen && e.isLoading]
-                ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
+                ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
-                    class: (0, s.C_)(["camera-box", {
+                    class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
-                }, [(0, l._)("div", {
-                    class: (0, s.C_)(["camera-shutter", {
+                }, [(0, s._)("div", {
+                    class: (0, l.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
-                }, null, 2), (0, l.wy)((0, l._)("video", {
+                }, null, 2), (0, s.wy)((0, s._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, ye), [
+                }, null, 8, we), [
                     [ne.F8, !e.isPhotoTaken]
-                ]), (0, l.wy)((0, l._)("canvas", {
+                ]), (0, s.wy)((0, s._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
                 }, null, 8, be), [
                     [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
                     [ne.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", ke, [(0, l._)("button", {
+                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ke, [(0, s._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, xe)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", Ce, [(0, l.Wm)(C, {
+                }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(C, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(C, {
+                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(C, {
                     key: 17,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
-                    default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
+                    default: (0, s.w5)((() => [e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(q, {
                         key: 0,
                         class: "text-body2"
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
+                        default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
-                    })) : (0, l.kq)("", !0)])),
+                    })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(C, {
+                }, 8, ["label", "icon", "onClick"])) : ((0, s.wg)(), (0, s.j4)(C, {
                     key: 18,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
-                    default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
+                    default: (0, s.w5)((() => [e.data.tooltip ? ((0, s.wg)(), (0, s.j4)(q, {
                         key: 0,
                         class: "text-body2"
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
+                        default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
-                    })) : (0, l.kq)("", !0)])),
+                    })) : (0, s.kq)("", !0)])),
                     _: 1
                 }, 8, ["icon", "onClick"]))
             }
             const _e = {
                     key: 0
                 },
                 je = {
                     class: "row"
                 },
                 Se = ["onClick"];
 
             function ze(e, t, a, i, o, n) {
-                const d = (0, l.up)("q-icon"),
-                    r = (0, l.up)("q-tooltip"),
-                    c = (0, l.up)("q-input"),
-                    h = (0, l.up)("q-btn"),
-                    u = (0, l.up)("q-th"),
-                    p = (0, l.up)("q-tr"),
-                    g = (0, l.up)("q-checkbox"),
-                    m = (0, l.up)("q-select"),
-                    f = (0, l.up)("q-td"),
-                    w = (0, l.up)("q-table");
-                return (0, l.wg)(), (0, l.j4)(w, {
+                const d = (0, s.up)("q-icon"),
+                    r = (0, s.up)("q-tooltip"),
+                    c = (0, s.up)("q-input"),
+                    h = (0, s.up)("q-btn"),
+                    u = (0, s.up)("q-th"),
+                    p = (0, s.up)("q-tr"),
+                    g = (0, s.up)("q-checkbox"),
+                    m = (0, s.up)("q-select"),
+                    f = (0, s.up)("q-td"),
+                    y = (0, s.up)("q-table");
+                return (0, s.wg)(), (0, s.j4)(y, {
                     class: "my-sticky-virtscroll-table",
                     "virtual-scroll": "",
                     dense: "",
-                    style: (0, s.j5)(e.styleSize),
+                    style: (0, l.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
                     virtualScrollSliceSize: "60",
                     "rows-per-page-options": [0],
                     "virtual-scroll-sticky-size-start": 48,
                     "row-key": "iiid",
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l._)("div", je, [(0, l.Wm)(c, {
+                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", _e, [(0, s._)("div", je, [(0, s.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
-                    }, (0, l.Nv)({
-                        append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
+                    }, (0, s.Nv)({
+                        append: (0, s.w5)((() => ["" != e.search ? ((0, s.wg)(), (0, s.j4)(d, {
                             key: 0,
                             class: "cursor-pointer",
                             name: "close",
                             size: "xs",
                             onClick: t[0] || (t[0] = t => {
                                 e.search = "", e.$refs.searchField.focus()
                             })
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                            default: (0, s.w5)((() => [(0, s.Wm)(r, {
                                 class: "text-body2"
                             }, {
-                                default: (0, l.w5)((() => [(0, l.Uk)("Reset search")])),
+                                default: (0, s.w5)((() => [(0, s.Uk)("Reset search")])),
                                 _: 1
                             })])),
                             _: 1
-                        })) : (0, l.kq)("", !0)])),
+                        })) : (0, s.kq)("", !0)])),
                         _: 2
                     }, ["" == e.search ? {
                         name: "prepend",
-                        fn: (0, l.w5)((() => [(0, l.Wm)(d, {
+                        fn: (0, s.w5)((() => [(0, s.Wm)(d, {
                             name: "search",
                             size: "xs"
                         })])),
                         key: "0"
-                    } : void 0]), 1032, ["modelValue"]), (0, l._)("div", null, [(0, l.Wm)(h, {
+                    } : void 0]), 1032, ["modelValue"]), (0, s._)("div", null, [(0, s.Wm)(h, {
                         dense: "",
                         rounded: "",
                         icon: "select_all",
                         "no-caps": "",
                         onClick: e.showSelected
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Show selected")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Show selected")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["onClick"]), (0, l.Wm)(h, {
+                    }, 8, ["onClick"]), (0, s.Wm)(h, {
                         dense: "",
                         rounded: "",
                         icon: "deselect",
                         "no-caps": "",
                         onClick: e.deselectAll
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Deselect all")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Deselect all")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["onClick"]), "delete" in e.data ? ((0, l.wg)(), (0, l.j4)(h, {
+                    }, 8, ["onClick"]), "delete" in e.data ? ((0, s.wg)(), (0, s.j4)(h, {
                         key: 0,
                         dense: "",
                         rounded: "",
                         icon: "delete_forever",
                         "no-caps": "",
                         onClick: e.delSelected
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Delete selected")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Delete selected")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["onClick"])) : (0, l.kq)("", !0), !1 !== e.data.multimode ? ((0, l.wg)(), (0, l.j4)(h, {
+                    }, 8, ["onClick"])) : (0, s.kq)("", !0), !1 !== e.data.multimode ? ((0, s.wg)(), (0, s.j4)(h, {
                         key: 1,
                         dense: "",
                         rounded: "",
                         icon: e.singleMode ? "looks_one" : "grain",
                         "no-caps": "",
                         onClick: e.switchMode
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Multi-single select mode")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Multi-single select mode")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["icon", "onClick"])) : (0, l.kq)("", !0), e.editable ? ((0, l.wg)(), (0, l.j4)(h, {
+                    }, 8, ["icon", "onClick"])) : (0, s.kq)("", !0), e.editable ? ((0, s.wg)(), (0, s.j4)(h, {
                         key: 2,
                         dense: "",
                         rounded: "",
                         icon: e.editMode ? "cancel" : "edit",
                         "no-caps": "",
                         onClick: e.switchEdit
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Edit mode")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Edit mode")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["icon", "onClick"])) : (0, l.kq)("", !0), e.editable && "append" in e.data ? ((0, l.wg)(), (0, l.j4)(h, {
+                    }, 8, ["icon", "onClick"])) : (0, s.kq)("", !0), e.editable && "append" in e.data ? ((0, s.wg)(), (0, s.j4)(h, {
                         key: 3,
                         dense: "",
                         rounded: "",
                         icon: "add",
                         "no-caps": "",
                         onClick: e.append
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Add a new row")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Add a new row")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["onClick"])) : (0, l.kq)("", !0), "view" in e.data ? ((0, l.wg)(), (0, l.j4)(h, {
+                    }, 8, ["onClick"])) : (0, s.kq)("", !0), "view" in e.data ? ((0, s.wg)(), (0, s.j4)(h, {
                         key: 4,
                         dense: "",
                         rounded: "",
                         icon: "insights",
                         "no-caps": "",
                         onClick: e.chart
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, s.w5)((() => [(0, s.Wm)(r, {
                             class: "text-body2"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)("Draw the chart")])),
+                            default: (0, s.w5)((() => [(0, s.Uk)("Draw the chart")])),
                             _: 1
                         })])),
                         _: 1
-                    }, 8, ["onClick"])) : (0, l.kq)("", !0)])])])) : (0, l.kq)("", !0)])),
-                    header: (0, l.w5)((e => [(0, l.Wm)(p, {
+                    }, 8, ["onClick"])) : (0, s.kq)("", !0)])])])) : (0, s.kq)("", !0)])),
+                    header: (0, s.w5)((e => [(0, s.Wm)(p, {
                         props: e
                     }, {
-                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.cols, (t => ((0, l.wg)(), (0, l.j4)(u, {
+                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.cols, (t => ((0, s.wg)(), (0, s.j4)(u, {
                             class: "text-italic text-purple",
                             key: t.name,
                             props: e
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(t.label), 1)])),
+                            default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(t.label), 1)])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props"])])),
-                    body: (0, l.w5)((t => [(0, l.Wm)(p, {
+                    body: (0, s.w5)((t => [(0, s.Wm)(p, {
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
-                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.columns, ((a, i) => ((0, l.wg)(), (0, l.j4)(f, {
+                        default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(f, {
                             key: a.name,
                             props: t
                         }, {
-                            default: (0, l.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, l.wg)(), (0, l.j4)(g, {
+                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(g, {
                                 key: 0,
                                 modelValue: t.row[a.name],
-                                "onUpdate:modelValue": [e => t.row[a.name] = e, l => e.change_switcher(t.row, a.name, i)],
+                                "onUpdate:modelValue": [e => t.row[a.name] = e, s => e.change_switcher(t.row, a.name, i)],
                                 dense: "",
                                 disable: !e.editMode
-                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(m, {
+                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(m, {
                                 key: 1,
                                 dense: "",
                                 "model-value": t.row[a.name],
                                 "use-input": "",
                                 "hide-selected": "",
                                 "fill-input": "",
                                 autofocus: "",
@@ -1034,79 +1034,79 @@
                                 borderless: "",
                                 onInputValue: e.change,
                                 "hide-dropdown-icon": "",
                                 "input-debounce": "0",
                                 options: e.options,
                                 onFilter: e.complete,
                                 onKeydown: e.keyInput
-                            }, null, 8, ["model-value", "onInputValue", "options", "onFilter", "onKeydown"])) : e.editMode && i == e.cedit && e.redit == t.row.iiid ? ((0, l.wg)(), (0, l.j4)(c, {
+                            }, null, 8, ["model-value", "onInputValue", "options", "onFilter", "onKeydown"])) : e.editMode && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(c, {
                                 key: 2,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
-                            }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
+                            }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, s.wg)(), (0, s.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, Se))])),
+                            }, (0, l.zw)(t.row[a.name]), 9, Se))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
             var Ae = a(1959);
 
             function Ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const Me = (0, l.aZ)({
+            const Me = (0, s.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
                     } = (0, Ae.BK)(e);
-                    let s = (0, l.Fl)((() => {
+                    let l = (0, s.Fl)((() => {
                             let e = [],
                                 a = t.value;
-                            const l = a.headers,
-                                s = l.length,
+                            const s = a.headers,
+                                l = s.length,
                                 i = a.rows,
                                 o = i.length;
                             for (var n = 0; n < o; n++) {
                                 const t = {},
                                     a = i[n];
-                                for (var d = 0; d < s; d++) t[l[d]] = a[d];
+                                for (var d = 0; d < l; d++) t[s[d]] = a[d];
                                 t.iiid = n, e.push(t)
                             }
                             return e
                         })),
                         i = () => {
                             let e = t.value,
-                                a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
+                                a = null === e.value || 0 == l.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => l.value[e])) : [l.value[e.value]];
                             return a
                         },
                         o = i(),
                         n = (0, Ae.iH)(o),
                         d = (0, Ae.iH)(o),
                         r = (0, Ae.iH)(!Array.isArray(t.value.value)),
-                        c = (e, l) => {
-                            q([a.value.name, t.value.name, e, l])
+                        c = (e, s) => {
+                            q([a.value.name, t.value.name, e, s])
                         },
-                        h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
-                        u = (0, l.Fl)((() => t.value.value));
-                    return (0, l.YP)(s, ((e, t) => {
+                        h = (0, s.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
+                        u = (0, s.Fl)((() => t.value.value));
+                    return (0, s.YP)(l, ((e, t) => {
                         d.value = i(), n.value = d.value
-                    })), (0, l.YP)(t, ((e, a) => {
+                    })), (0, s.YP)(t, ((e, a) => {
                         g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
-                        rows: s,
+                        rows: l,
                         value: h,
                         selected: d,
                         singleMode: r,
                         sendMessage: c,
                         datavalue: u,
                         updated: n
                     }
@@ -1122,18 +1122,18 @@
                 methods: {
                     select(e, t) {
                         this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
-                            const l = e.iiid;
-                            let s = this.data.rows;
-                            s[l][a] = e[t], this.sendMessage("#", [e[t],
-                                [l, a]
+                            const s = e.iiid;
+                            let l = this.data.rows;
+                            l[s][a] = e[t], this.sendMessage("#", [e[t],
+                                [s, a]
                             ])
                         }
                     },
                     change(e) {
                         if (g && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
                             let a = this.data.rows;
@@ -1195,17 +1195,17 @@
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        A(this, [t, this.search], (function(l) {
-                            if (!Array.isArray(l)) return u.error(l);
-                            g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
+                        A(this, [t, this.search], (function(s) {
+                            if (!Array.isArray(s)) return u.error(s);
+                            g && console.log("added row", s), a.search = "", e.push(s), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "+")
                     },
                     showSelected() {
                         let e = this.$refs.table;
@@ -1238,15 +1238,19 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        Ze(this.updated, this.selected) || (this.sendMessage("=", this.selected.length ? this.selected[0].iiid : null), this.updated = this.selected), t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
+                        if (!Ze(this.updated, this.selected)) {
+                            let e = this.selected.length;
+                            this.sendMessage("=", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
+                        }
+                        t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1270,138 +1274,151 @@
                     pdata: Object,
                     styleSize: String
                 }
             });
             var De = a(9267),
                 $e = a(4842),
                 Ve = a(8870),
-                Oe = a(2165),
-                Qe = a(8186),
-                We = a(2414),
-                He = a(3884),
-                Ee = a(5735),
-                Ue = a(7208);
-            const Ne = (0, N.Z)(Me, [
+                Ke = a(2165),
+                Oe = a(8186),
+                Ee = a(2414),
+                Qe = a(3884),
+                We = a(5735),
+                He = a(7208);
+            const Ue = (0, U.Z)(Me, [
                     ["render", ze]
                 ]),
-                Fe = Ne;
+                Ne = Ue;
             R()(Me, "components", {
                 QTable: De.Z,
                 QInput: $e.Z,
                 QIcon: P.Z,
                 QTooltip: Ve.Z,
-                QBtn: Oe.Z,
-                QTr: Qe.Z,
-                QTh: We.Z,
-                QTd: He.Z,
-                QCheckbox: Ee.Z,
-                QSelect: Ue.Z
+                QBtn: Ke.Z,
+                QTr: Oe.Z,
+                QTh: Ee.Z,
+                QTd: Qe.Z,
+                QCheckbox: We.Z,
+                QSelect: He.Z
             });
-            const Ke = ["nodes", "edges"];
+            const Fe = ["nodes", "edges"];
 
             function Pe(e, t, a, i, o, n) {
-                return (0, l.wg)(), (0, l.iD)("div", {
+                return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
-                    style: (0, s.j5)(e.styleSize),
+                    style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Ke)
+                }, null, 12, Fe)
             }
             var Te = a(2393),
                 Ie = a.n(Te);
             const Re = Ie().stylesheet().selector("node").css({
                     content: "data(id)",
-                    "background-color": "#4286f4"
+                    "background-color": "#4286f4",
+                    "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
-                    "border-color": "#ff5555"
+                    "border-color": "#ff5555",
+                    "font-size": "14px"
                 }).selector("node[label]").css({
                     label: "data(label)",
                     "text-valign": "bottom",
-                    "text-halign": "center"
+                    "text-halign": "center",
+                    "font-size": "14px"
                 }).selector("edge").css({
                     label: "data(label)",
                     "curve-style": "bezier",
                     "target-arrow-shape": "triangle",
                     width: 4,
                     "line-color": "#4286f4",
-                    "target-arrow-color": "#4286f4"
+                    "target-arrow-color": "#4286f4",
+                    "font-size": "12px"
                 }).selector(".highlighted").css({
                     "line-color": "pink",
-                    "target-arrow-color": "#b830f7"
+                    "target-arrow-color": "#b830f7",
+                    "font-size": "12px"
                 }).selector("edge[label]").css({
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
-                    color: "gray"
+                    color: "gray",
+                    "font-size": "12px"
                 }),
-                Be = {
+                Le = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Le(e, t) {
+            function Be(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
-                    if (e[a].id != t[a].id) return !0;
+                    if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Ye = (0, l.aZ)({
+            const Ye = (0, s.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
                             style: Re,
-                            layoutOptions: Be,
+                            layoutOptions: Le,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
-                            oldEdges: []
+                            oldEdges: [],
+                            shiftKey: !1
                         }
                     },
+                    beforeUnmount() {
+                        window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
+                    },
                     mounted() {
+                        window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
                         let e = Ie()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
                             t = this.value.nodes;
                         this.selectedNodes = t || [];
-                        for (let s of this.selectedNodes) e.nodes("[id='" + s + "']").addClass("selected");
+                        for (let l of this.selectedNodes) e.nodes("[id='" + l + "']").addClass("selected");
                         let a = this.value.edges;
                         this.selectedEdges = a || [];
-                        for (let s of this.selectedEdges) e.edges("[id='" + s + "']").addClass("highlighted");
+                        for (let l of this.selectedEdges) e.edges("[id='" + l + "']").addClass("highlighted");
                         this.cy = e;
-                        let l = this;
+                        let s = this;
                         e.on("tap", "node", (t => {
                             const a = t.target;
                             if (a.hasClass("selected")) {
                                 a.removeClass("selected");
                                 let e = a.id();
-                                l.selectedNodes = l.selectedNodes.filter((t => t !== e))
-                            } else l.selectedNodes.length > 0 && (e.$(".selected").removeClass("selected"), l.selectedNodes = []), l.selectedEdges.length > 0 && (e.$(".selected").removeClass("selected"), l.selectedEdges = []), a.addClass("selected"), l.selectedNodes.push(a.id());
-                            l.sendMessage("=", {
-                                nodes: l.selectedNodes
+                                s.selectedNodes = s.shiftKey ? s.selectedNodes.filter((t => t !== e)) : []
+                            } else !s.shiftKey && s.selectedEdges.length > 0 && (e.$(".selected").removeClass("selected"), s.selectedEdges = []), a.addClass("selected"), s.selectedNodes.push(a.id());
+                            s.sendMessage("=", {
+                                nodes: s.selectedNodes,
+                                edges: s.selectedEdges
                             })
                         })), e.on("click", (function(t) {
                             let a = t.target;
-                            if (a === e || "edges" == t.target.group()) {
-                                e.edges().removeClass("highlighted");
+                            if ("id" in a && (a === e || "edges" == t.target.group())) {
+                                s.shiftKey || e.edges().removeClass("highlighted");
                                 let t = a.id();
-                                l.selectedEdges.includes(t) ? l.selectedEdges = [] : (e.edges("[id='" + t + "']").addClass("highlighted"), l.selectedEdges = [t]), l.sendMessage("=", {
-                                    edges: l.selectedEdges
+                                s.selectedEdges.includes(t) ? (s.selectedEdges = s.shiftKey ? s.selectedEdges.filter((e => e != t)) : [], e.edges("[id='" + t + "']").removeClass("highlighted")) : (e.edges("[id='" + t + "']").addClass("highlighted"), s.shiftKey ? s.selectedEdges.push(t) : s.selectedEdges = [t]), s.sendMessage("=", {
+                                    nodes: s.selectedNodes,
+                                    edges: s.selectedEdges
                                 })
                             }
                         }))
                     },
                     computed: {
                         nodes() {
                             return this.data.nodes.map((e => ({
@@ -1419,19 +1436,25 @@
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
                             q([this.pdata["name"], this.data["name"], e, t])
                         },
+                        handleKeyDown(e) {
+                            "Shift" == e.key && (this.shiftKey = !0), console.log(this.shiftKey)
+                        },
+                        handleKeyUp(e) {
+                            "Shift" == e.key && (this.shiftKey = !1), console.log(this.shiftKey)
+                        },
                         showClusterNode(e) {
                             const t = e.data("cluster"),
                                 a = this.cy.nodes(`[cluster='${t}']`),
-                                l = this.cy.nodes(`#${t}`);
-                            l.data("isClusterNode", !0), l.animate({
+                                s = this.cy.nodes(`#${t}`);
+                            s.data("isClusterNode", !0), s.animate({
                                 position: {
                                     x: e.position("x"),
                                     y: e.position("y")
                                 },
                                 width: a.boundingBox().w,
                                 height: a.boundingBox().h,
                                 duration: 300
@@ -1483,16 +1506,16 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 console.log("wa gr");
                                 let a = e.value,
-                                    l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Le(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Le(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                    s = !1;
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1509,41 +1532,41 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Xe = (0, N.Z)(Ye, [
+                Xe = (0, U.Z)(Ye, [
                     ["render", Pe]
                 ]),
                 Ge = Xe;
 
             function Je(e, t, a, i, o, n) {
-                const d = (0, l.up)("v-chart");
-                return (0, l.wg)(), (0, l.j4)(d, {
+                const d = (0, s.up)("v-chart");
+                return (0, s.wg)(), (0, s.j4)(d, {
                     ref: "chart",
                     option: o.options,
-                    style: (0, s.j5)(a.styleSize),
+                    style: (0, l.j5)(a.styleSize),
                     autoresize: !0,
                     onClick: n.clicked
                 }, null, 8, ["option", "style", "onClick"])
             }
             var et = a(5512),
                 tt = a(4447),
                 at = a(1006),
-                lt = a(3526),
-                st = a(763),
+                st = a(3526),
+                lt = a(763),
                 it = a(546),
                 ot = a(6902),
                 nt = a(2826),
                 dt = a(5256),
                 rt = a(3825),
                 ct = a(8825);
-            (0, st.D)([tt.N, at.N, lt.N]), (0, st.D)([it.N, ot.N, nt.N, dt.N, rt.N]);
+            (0, lt.D)([tt.N, at.N, st.N]), (0, lt.D)([it.N, ot.N, nt.N, dt.N, rt.N]);
             let ht = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
                 ut = {
                     responsive: !0,
                     maintainAspectRatio: !1,
                     legend: {
                         data: [],
                         bottom: 10
@@ -1602,16 +1625,16 @@
                             options: null
                         }
                     },
                     methods: {
                         clicked(e) {
                             var t = [e.offsetX, e.offsetY],
                                 a = myChart.convertFromPixel("grid", t),
-                                l = myChart.getModel().get("xAxis")[0].data[a[0]];
-                            console.log(l)
+                                s = myChart.getModel().get("xAxis")[0].data[a[0]];
+                            console.log(s)
                         },
                         calcSeries() {
                             this.options.toolbox.feature.mySwitcher = {
                                 show: !0,
                                 title: "Switch view to the table",
                                 icon: "image:M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm15 2h-4v3h4V4zm0 4h-4v3h4V8zm0 4h-4v3h3a1 1 0 0 0 1-1v-2zm-5 3v-3H6v3h4zm-5 0v-3H1v2a1 1 0 0 0 1 1h3zm-4-4h4V8H1v3zm0-4h4V4H1v3zm5-3v3h4V4H6zm4 4H6v3h4V8z",
                                 onclick: () => {
@@ -1619,56 +1642,56 @@
                                     e.type = "table"
                                 }
                             };
                             let e = this.data.view,
                                 t = this.data.headers;
                             "_" != this.data.name[0] && (this.options.title.text = this.data.name);
                             let a = e.split("-"),
-                                l = a[1].split(",");
-                            l.unshift(a[0]);
-                            let s = [];
-                            for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
-                                name: t[l[o]],
+                                s = a[1].split(",");
+                            s.unshift(a[0]);
+                            let l = [];
+                            for (let o = 0; o < s.length; o++) s[o] = "i" == s[o] ? -1 : parseInt(s[o]), l.push([]), o && (this.options.series.push({
+                                name: t[s[o]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
                                     color: ht[o]
                                 },
-                                data: s[o]
-                            }), this.options.legend.data.push(t[l[o]]));
-                            this.options.xAxis.data = s[0];
+                                data: l[o]
+                            }), this.options.legend.data.push(t[s[o]]));
+                            this.options.xAxis.data = l[0];
                             let i = this.data.rows;
                             for (let o = 0; o < i.length; o++)
-                                for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
+                                for (let e = 0; e < s.length; e++) l[e].push(-1 == s[e] ? o : i[o][s[e]]);
                             this.$refs.chart.setOption(this.options)
                         }
                     },
                     mounted() {
                         this.options = (0, h.cloneDeep)(ut), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
                     },
                     watch: {}
                 },
-                gt = (0, N.Z)(pt, [
+                gt = (0, U.Z)(pt, [
                     ["render", Je]
                 ]),
                 mt = gt;
 
             function ft(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const wt = (0, l.aZ)({
+            const yt = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Fe,
+                    utable: Ne,
                     cgraph: Ge,
                     linechart: mt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
@@ -1679,15 +1702,15 @@
                         q([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("->", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("=", e.files[t - 1].name), Q())
+                        t && (this.sendMessage("=", e.files[t - 1].name), O())
                     },
                     sendValue() {
                         this.sendMessage("=", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
@@ -1739,33 +1762,33 @@
                         document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
-                            l = e.getBoundingClientRect();
+                            s = e.getBoundingClientRect();
                         return {
                             el: e,
                             inner: a,
-                            left: l.left,
-                            right: l.right,
-                            top: l.top,
+                            left: s.left,
+                            right: s.right,
+                            top: s.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
                     k[this.fullname] = this, g && console.log("mounted", this.fullname)
                 },
                 data() {
                     return {
                         value: this.data.value,
-                        styleSize: y(this.data),
+                        styleSize: w(this.data),
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -1833,25 +1856,25 @@
                     treeNodes() {
                         var e = [];
                         if ("list" == this.type) return this.data.options.map((e => ({
                             label: e,
                             children: []
                         })));
                         var t = {};
-                        for (const [s, i] of Object.entries(this.data.options)) {
-                            var a = t[s];
+                        for (const [l, i] of Object.entries(this.data.options)) {
+                            var a = t[l];
                             if (a || (a = {
-                                    label: s,
+                                    label: l,
                                     children: []
-                                }, t[s] = a), i) {
-                                var l = t[i];
-                                l || (l = {
+                                }, t[l] = a), i) {
+                                var s = t[i];
+                                s || (s = {
                                     label: i,
                                     children: []
-                                }, t[i] = l), l.children.push(a)
+                                }, t[i] = s), s.children.push(a)
                             } else e.push(a)
                         }
                         return e
                     }
                 },
                 props: {
                     data: {
@@ -1871,55 +1894,55 @@
                         g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        g && console.log("data update", this.fullname, t.name), this.styleSize || (this.styleSize = y(this.data), g && console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
+                        g && console.log("data update", this.fullname, t.name), this.styleSize || (this.styleSize = w(this.data), g && console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var yt = a(4027),
+            var wt = a(4027),
                 bt = a(9721),
                 kt = a(8886),
                 vt = a(8761),
                 xt = a(1232),
                 Ct = a(5551),
                 qt = a(5869),
                 _t = a(1745);
-            const jt = (0, N.Z)(wt, [
+            const jt = (0, U.Z)(yt, [
                     ["render", qe],
                     ["__scopeId", "data-v-606d07c3"]
                 ]),
                 St = jt;
-            R()(wt, "components", {
-                QImg: yt.Z,
+            R()(yt, "components", {
+                QImg: wt.Z,
                 QIcon: P.Z,
-                QSelect: Ue.Z,
+                QSelect: He.Z,
                 QBadge: bt.Z,
-                QCheckbox: Ee.Z,
+                QCheckbox: We.Z,
                 QToggle: kt.Z,
                 QBtnToggle: vt.Z,
                 QInput: $e.Z,
                 QScrollArea: xt.Z,
                 QTree: Ct.Z,
                 QSeparator: qt.Z,
                 QUploader: _t.Z,
-                QBtn: Oe.Z,
+                QBtn: Ke.Z,
                 QTooltip: Ve.Z
             });
-            const zt = (0, l.aZ)({
+            const zt = (0, s.aZ)({
                 name: "block",
                 components: {
                     element: St
                 },
                 data() {
                     return {
-                        styleSize: w,
+                        styleSize: y,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
                         },
@@ -1978,90 +2001,90 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), this.styleSize = w, b[this.name] = this, this.expanding && (k[this.fullname] = this)
+                        g && console.log("data update", this.name), this.styleSize = y, b[this.name] = this, this.expanding && (k[this.fullname] = this)
                     }
                 }
             });
             var At = a(151);
-            const Zt = (0, N.Z)(zt, [
+            const Zt = (0, U.Z)(zt, [
                     ["render", oe]
                 ]),
                 Mt = Zt;
             R()(zt, "components", {
                 QCard: At.Z,
                 QIcon: P.Z,
                 QScrollArea: xt.Z
             });
-            const Dt = (0, l.aZ)({
+            const Dt = (0, s.aZ)({
                     name: "zone",
                     components: {
                         block: Mt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
-                        (0, l.Y3)((() => {
+                        (0, s.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
-                                    W()
+                                    E()
                                 }))
                             }))
                         }))
                     }
                 }),
-                $t = (0, N.Z)(Dt, [
+                $t = (0, U.Z)(Dt, [
                     ["render", J]
                 ]),
                 Vt = $t,
-                Ot = {
+                Kt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Qt(e, t, a, i, o, n) {
-                const d = (0, l.up)("block"),
-                    r = (0, l.up)("q-item-label"),
-                    c = (0, l.up)("q-space"),
-                    h = (0, l.up)("q-btn"),
-                    u = (0, l.up)("q-card"),
-                    p = (0, l.up)("q-dialog");
-                return (0, l.wg)(), (0, l.j4)(p, {
+            function Ot(e, t, a, i, o, n) {
+                const d = (0, s.up)("block"),
+                    r = (0, s.up)("q-item-label"),
+                    c = (0, s.up)("q-space"),
+                    h = (0, s.up)("q-btn"),
+                    u = (0, s.up)("q-card"),
+                    p = (0, s.up)("q-dialog");
+                return (0, s.wg)(), (0, s.j4)(p, {
                     ref: "dialog",
                     onHide: n.onDialogHide
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(u, {
+                    default: (0, s.w5)((() => [(0, s.Wm)(u, {
                         class: "q-dialog-plugin q-pa-md items-start q-gutter-md",
                         bordered: "",
-                        style: (0, s.j5)(a.data.internal ? "width: 800px; max-width: 80vw;" : "")
+                        style: (0, l.j5)(a.data.internal ? "width: 800px; max-width: 80vw;" : "")
                     }, {
-                        default: (0, l.w5)((() => [a.data ? ((0, l.wg)(), (0, l.j4)(d, {
+                        default: (0, s.w5)((() => [a.data ? ((0, s.wg)(), (0, s.j4)(d, {
                             key: 0,
                             data: a.data
-                        }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
+                        }, null, 8, ["data"])) : (0, s.kq)("", !0), (0, s.Wm)(r, {
                             class: "text-h6"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
+                            default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Ot, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, s._)("div", Kt, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const Wt = {
+            const Et = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
                     block: Mt
                 },
@@ -2083,30 +2106,30 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Ht = a(5926),
-                Et = a(2025);
-            const Ut = (0, N.Z)(Wt, [
-                    ["render", Qt]
+            var Qt = a(5926),
+                Wt = a(2025);
+            const Ht = (0, U.Z)(Et, [
+                    ["render", Ot]
                 ]),
-                Nt = Ut;
-            R()(Wt, "components", {
-                QDialog: Ht.Z,
+                Ut = Ht;
+            R()(Et, "components", {
+                QDialog: Qt.Z,
                 QCard: At.Z,
                 QItemLabel: T.Z,
-                QSpace: Et.Z,
-                QBtn: Oe.Z
+                QSpace: Wt.Z,
+                QBtn: Ke.Z
             });
-            var Ft = !0;
-            let Kt = null;
-            const Pt = (0, l.aZ)({
+            var Nt = !0;
+            let Ft = null;
+            const Pt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         data: {
@@ -2116,15 +2139,15 @@
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
-                    menubar: L,
+                    menubar: B,
                     zone: Vt,
                     element: St
                 },
                 created() {
                     C(this)
                 },
                 unmounted() {
@@ -2134,116 +2157,116 @@
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         q(["root", e])
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), Q()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), O()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Nt
+                                component: Ut
                             },
                             {
                                 height: a,
-                                ...l
+                                ...s
                             } = e;
-                        l.width = 750;
-                        let s = {
+                        s.width = 750;
+                        let l = {
                             name: `Picture lens of ${e.name}`,
                             top_childs: [],
-                            childs: [l],
+                            childs: [s],
                             internal: !0
                         };
                         t.componentProps = {
-                            data: s,
+                            data: l,
                             buttons: ["Close"]
                         }, this.$q.dialog(t)
                     },
                     notify(e, t) {
                         let a = t,
-                            l = {
+                            s = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Kt ? (l = {
+                        "progress" == t ? null == Ft ? (s = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Kt = this.$q.notify(l)) : null == e ? (Kt(), Kt = null) : (l = {
+                        }, Ft = this.$q.notify(s)) : null == e ? (Ft(), Ft = null) : (s = {
                             caption: e
-                        }, Kt(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Ft(s)) : ("error" == t && s.type, this.$q.notify(s))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (Ft) Ft = !1, this.menu = e[0].map((e => ({
+                        if (Nt) Nt = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
                         else if ("screen" == e.type) this.screen.name != e.name && z(), Z(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Nt, t.componentProps = {
+                            t.component = Ut, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if (e.hasOwnProperty("answer")) $(e);
                         else {
                             e.update && D(e);
                             let t = !1;
                             for (let a of v) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Kt && !e.progress && this.notify(null, "progress")
+                        Ft && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
             var Tt = a(9214),
                 It = a(3812),
                 Rt = a(9570),
-                Bt = a(7547),
-                Lt = a(3269),
+                Lt = a(7547),
+                Bt = a(3269),
                 Yt = a(2652),
                 Xt = a(4379);
-            const Gt = (0, N.Z)(Pt, [
+            const Gt = (0, U.Z)(Pt, [
                     ["render", n]
                 ]),
                 Jt = Gt;
             R()(Pt, "components", {
                 QLayout: Tt.Z,
                 QHeader: It.Z,
                 QToolbar: Rt.Z,
-                QBtn: Oe.Z,
+                QBtn: Ke.Z,
                 QItemLabel: T.Z,
-                QTabs: Bt.Z,
-                QTab: Lt.Z,
+                QTabs: Lt.Z,
+                QTab: Bt.Z,
                 QPageContainer: Yt.Z,
                 QPage: Xt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.7.0/unigui/web/js/app.59c7eb11.js` & `unigui-1.7.1/unigui/web/js/app.feb97290.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(274)]).then(r.bind(r, 9274)),
+                        component: () => Promise.all([r.e(736), r.e(572)]).then(r.bind(r, 5572)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            274: "9d2f3775",
-            430: "591e9a73"
+            430: "591e9a73",
+            572: "4a65c656"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            274: "13cee13e",
+            572: "13cee13e",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                274: 1
+                572: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.7.0/unigui/web/js/193.283445be.js` & `unigui-1.7.1/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.7.1/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/unigui/web/index.html` & `unigui-1.7.1/unigui/web/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.59c7eb11.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.feb97290.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.7.0/LICENSE` & `unigui-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.7.0/setup.py` & `unigui-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.7.0',      
+      version='1.7.1',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.7.0/PKG-INFO` & `unigui-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.7.0
+Version: 1.7.1
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -348,14 +348,15 @@
 def graph_selection(_, val):
     _.value = val
     if 'nodes' in val:        
         return Info(f'Nodes {val["nodes"]}') 
     if 'edges' in val:
         return Info(f"Edges {val['edges']}") 
 ```
+With pressed 'Shift' multi select works for nodes and edges.
 
 Has optional draw 'method' with options 'random', 'circle', 'breadthfirst', by default 'random'.
 
 ### Dialog ###
 ```
 Dialog(name, text, callback, buttons, content = None)
 ```
@@ -412,8 +413,10 @@
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
 
+Unigui protocol messages from/to server you can see in a browser console (F12).
+
```

### Comparing `unigui-1.7.0/README.md` & `unigui-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -336,14 +336,15 @@
 def graph_selection(_, val):
     _.value = val
     if 'nodes' in val:        
         return Info(f'Nodes {val["nodes"]}') 
     if 'edges' in val:
         return Info(f"Edges {val['edges']}") 
 ```
+With pressed 'Shift' multi select works for nodes and edges.
 
 Has optional draw 'method' with options 'random', 'circle', 'breadthfirst', by default 'random'.
 
 ### Dialog ###
 ```
 Dialog(name, text, callback, buttons, content = None)
 ```
@@ -399,7 +400,9 @@
 ```
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
+
+Unigui protocol messages from/to server you can see in a browser console (F12).
```

### Comparing `unigui-1.7.0/unigui.egg-info/PKG-INFO` & `unigui-1.7.1/unigui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.7.0
+Version: 1.7.1
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -348,14 +348,15 @@
 def graph_selection(_, val):
     _.value = val
     if 'nodes' in val:        
         return Info(f'Nodes {val["nodes"]}') 
     if 'edges' in val:
         return Info(f"Edges {val['edges']}") 
 ```
+With pressed 'Shift' multi select works for nodes and edges.
 
 Has optional draw 'method' with options 'random', 'circle', 'breadthfirst', by default 'random'.
 
 ### Dialog ###
 ```
 Dialog(name, text, callback, buttons, content = None)
 ```
@@ -412,8 +413,10 @@
 print(isinstance(user, Hello_user))
 ```
 
 More info about User class methods you can find in manager.py in the souce dir.
 
 Examples are in tests folder.
 
+Unigui protocol messages from/to server you can see in a browser console (F12).
+
```

### Comparing `unigui-1.7.0/unigui.egg-info/SOURCES.txt` & `unigui-1.7.1/unigui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/274.13cee13e.css
+unigui/web/css/572.13cee13e.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -27,11 +27,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/274.9d2f3775.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.59c7eb11.js
+unigui/web/js/572.4a65c656.js
+unigui/web/js/app.feb97290.js
 unigui/web/js/vendor.3e8714c2.js
```

