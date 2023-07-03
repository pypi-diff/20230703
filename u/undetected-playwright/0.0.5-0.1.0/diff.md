# Comparing `tmp/undetected-playwright-0.0.5.tar.gz` & `tmp/undetected-playwright-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undetected-playwright-0.0.5.tar", last modified: Mon Oct 24 11:36:39 2022, max compression
+gzip compressed data, was "undetected-playwright-0.1.0.tar", last modified: Mon Jul  3 06:04:03 2023, max compression
```

## Comparing `undetected-playwright-0.0.5.tar` & `undetected-playwright-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-10-24 11:36:39.471634 undetected-playwright-0.0.5/
--rw-rw-rw-   0        0        0    11558 2022-10-24 04:51:51.000000 undetected-playwright-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2166 2022-10-24 11:36:39.469627 undetected-playwright-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1373 2022-10-24 08:12:45.000000 undetected-playwright-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2022-10-24 11:36:39.472625 undetected-playwright-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1353 2022-10-24 08:50:13.000000 undetected-playwright-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-24 11:36:39.404651 undetected-playwright-0.0.5/undetected_playwright/
--rw-rw-rw-   0        0        0      291 2022-10-24 11:36:26.000000 undetected-playwright-0.0.5/undetected_playwright/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-24 11:36:39.466627 undetected-playwright-0.0.5/undetected_playwright/js/
--rw-rw-rw-   0        0        0     2091 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/chrome.app.js
--rw-rw-rw-   0        0        0     1013 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/chrome.csi.js
--rw-rw-rw-   0        0        0      483 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/chrome.hairline.js
--rw-rw-rw-   0        0        0     4522 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/chrome.load.times.js
--rw-rw-rw-   0        0        0     9846 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/chrome.runtime.js
--rw-rw-rw-   0        0        0     6583 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/generate.magic.arrays.js
--rw-rw-rw-   0        0        0     3662 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/iframe.contentWindow.js
--rw-rw-rw-   0        0        0     1749 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/media.codecs.js
--rw-rw-rw-   0        0        0      330 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.hardwareConcurrency.js
--rw-rw-rw-   0        0        0      243 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.languages.js
--rw-rw-rw-   0        0        0     1894 2022-10-24 07:56:42.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.permissions.js
--rw-rw-rw-   0        0        0      161 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.platform.js
--rw-rw-rw-   0        0        0     3461 2022-10-24 06:04:06.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.plugins.js
--rw-rw-rw-   0        0        0      501 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.userAgent.js
--rw-rw-rw-   0        0        0      129 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/navigator.vendor.js
--rw-rw-rw-   0        0        0        0 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/sourceurl.js
--rw-rw-rw-   0        0        0    18029 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/utils.js
--rw-rw-rw-   0        0        0      602 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/webdriver.js
--rw-rw-rw-   0        0        0     1174 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/webgl.vendor.js
--rw-rw-rw-   0        0        0      424 2022-10-23 13:36:25.000000 undetected-playwright-0.0.5/undetected_playwright/js/window.outerdimensions.js
--rw-rw-rw-   0        0        0     5399 2022-10-24 11:36:26.000000 undetected-playwright-0.0.5/undetected_playwright/ninja.py
-drwxrwxrwx   0        0        0        0 2022-10-24 11:36:39.416616 undetected-playwright-0.0.5/undetected_playwright.egg-info/
--rw-rw-rw-   0        0        0     2166 2022-10-24 11:36:39.000000 undetected-playwright-0.0.5/undetected_playwright.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2022-10-24 11:36:39.000000 undetected-playwright-0.0.5/undetected_playwright.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-24 11:36:39.000000 undetected-playwright-0.0.5/undetected_playwright.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2022-10-24 11:36:39.000000 undetected-playwright-0.0.5/undetected_playwright.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-10-24 11:36:39.000000 undetected-playwright-0.0.5/undetected_playwright.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 06:04:03.310131 undetected-playwright-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2022-10-24 04:51:51.000000 undetected-playwright-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2166 2023-07-03 06:04:03.309136 undetected-playwright-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1373 2022-10-24 08:12:45.000000 undetected-playwright-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:04:03.311135 undetected-playwright-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2023-07-03 06:03:21.000000 undetected-playwright-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:04:03.262422 undetected-playwright-0.1.0/undetected_playwright/
+-rw-rw-rw-   0        0        0      291 2023-07-03 06:03:57.000000 undetected-playwright-0.1.0/undetected_playwright/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:04:03.308137 undetected-playwright-0.1.0/undetected_playwright/js/
+-rw-rw-rw-   0        0        0     2091 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/chrome.app.js
+-rw-rw-rw-   0        0        0     1013 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/chrome.csi.js
+-rw-rw-rw-   0        0        0      483 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/chrome.hairline.js
+-rw-rw-rw-   0        0        0     4522 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/chrome.load.times.js
+-rw-rw-rw-   0        0        0     9846 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/chrome.runtime.js
+-rw-rw-rw-   0        0        0     6583 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/generate.magic.arrays.js
+-rw-rw-rw-   0        0        0     3662 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/iframe.contentWindow.js
+-rw-rw-rw-   0        0        0     1749 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/media.codecs.js
+-rw-rw-rw-   0        0        0      330 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.hardwareConcurrency.js
+-rw-rw-rw-   0        0        0      243 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.languages.js
+-rw-rw-rw-   0        0        0     1894 2022-10-24 07:56:42.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.permissions.js
+-rw-rw-rw-   0        0        0      161 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.platform.js
+-rw-rw-rw-   0        0        0     3461 2022-10-24 06:04:06.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.plugins.js
+-rw-rw-rw-   0        0        0      501 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.userAgent.js
+-rw-rw-rw-   0        0        0      129 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/navigator.vendor.js
+-rw-rw-rw-   0        0        0        0 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/sourceurl.js
+-rw-rw-rw-   0        0        0    18029 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/utils.js
+-rw-rw-rw-   0        0        0      602 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/webdriver.js
+-rw-rw-rw-   0        0        0     1174 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/webgl.vendor.js
+-rw-rw-rw-   0        0        0      424 2022-10-23 13:36:25.000000 undetected-playwright-0.1.0/undetected_playwright/js/window.outerdimensions.js
+-rw-rw-rw-   0        0        0     5399 2022-10-24 11:36:26.000000 undetected-playwright-0.1.0/undetected_playwright/ninja.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:04:03.270433 undetected-playwright-0.1.0/undetected_playwright.egg-info/
+-rw-rw-rw-   0        0        0     2166 2023-07-03 06:04:03.000000 undetected-playwright-0.1.0/undetected_playwright.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-07-03 06:04:03.000000 undetected-playwright-0.1.0/undetected_playwright.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:04:03.000000 undetected-playwright-0.1.0/undetected_playwright.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 06:04:03.000000 undetected-playwright-0.1.0/undetected_playwright.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-03 06:04:03.000000 undetected-playwright-0.1.0/undetected_playwright.egg-info/top_level.txt
```

### Comparing `undetected-playwright-0.0.5/LICENSE` & `undetected-playwright-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/PKG-INFO` & `undetected-playwright-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-playwright
-Version: 0.0.5
+Version: 0.1.0
 Summary: You know who I am
 Home-page: https://github.com/QIN2DIM/undetected-playwright
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 License: Apache-2.0 license
 Keywords: playwright,undetected-playwright,playwright-stealth
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `undetected-playwright-0.0.5/README.md` & `undetected-playwright-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/setup.py` & `undetected-playwright-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     url="https://github.com/QIN2DIM/undetected-playwright",
     license="Apache-2.0 license",
     author="QIN2DIM",
     author_email="yaoqinse@gmail.com",
     description="You know who I am",
     long_description=Path(__file__).parent.joinpath("README.md").read_text(),
     long_description_content_type="text/markdown",
-    install_requires=["playwright~=1.27.1"],
+    install_requires=["playwright"],
     python_requires=">=3.8",
     classifiers=[
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/chrome.app.js` & `undetected-playwright-0.1.0/undetected_playwright/js/chrome.app.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/chrome.csi.js` & `undetected-playwright-0.1.0/undetected_playwright/js/chrome.csi.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/chrome.load.times.js` & `undetected-playwright-0.1.0/undetected_playwright/js/chrome.load.times.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/chrome.runtime.js` & `undetected-playwright-0.1.0/undetected_playwright/js/chrome.runtime.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/generate.magic.arrays.js` & `undetected-playwright-0.1.0/undetected_playwright/js/generate.magic.arrays.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/iframe.contentWindow.js` & `undetected-playwright-0.1.0/undetected_playwright/js/iframe.contentWindow.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/media.codecs.js` & `undetected-playwright-0.1.0/undetected_playwright/js/media.codecs.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/navigator.permissions.js` & `undetected-playwright-0.1.0/undetected_playwright/js/navigator.permissions.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/navigator.plugins.js` & `undetected-playwright-0.1.0/undetected_playwright/js/navigator.plugins.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/utils.js` & `undetected-playwright-0.1.0/undetected_playwright/js/utils.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/webdriver.js` & `undetected-playwright-0.1.0/undetected_playwright/js/webdriver.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/js/webgl.vendor.js` & `undetected-playwright-0.1.0/undetected_playwright/js/webgl.vendor.js`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright/ninja.py` & `undetected-playwright-0.1.0/undetected_playwright/ninja.py`

 * *Files identical despite different names*

### Comparing `undetected-playwright-0.0.5/undetected_playwright.egg-info/PKG-INFO` & `undetected-playwright-0.1.0/undetected_playwright.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undetected-playwright
-Version: 0.0.5
+Version: 0.1.0
 Summary: You know who I am
 Home-page: https://github.com/QIN2DIM/undetected-playwright
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 License: Apache-2.0 license
 Keywords: playwright,undetected-playwright,playwright-stealth
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `undetected-playwright-0.0.5/undetected_playwright.egg-info/SOURCES.txt` & `undetected-playwright-0.1.0/undetected_playwright.egg-info/SOURCES.txt`

 * *Files identical despite different names*

