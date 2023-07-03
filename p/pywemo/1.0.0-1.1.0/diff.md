# Comparing `tmp/pywemo-1.0.0.tar.gz` & `tmp/pywemo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywemo-1.0.0.tar", max compression
+gzip compressed data, was "pywemo-1.1.0.tar", max compression
```

## Comparing `pywemo-1.0.0.tar` & `pywemo-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     2831 2023-06-17 22:27:32.227857 pywemo-1.0.0/LICENSE
--rw-r--r--   0        0        0     7620 2023-06-17 22:27:32.227857 pywemo-1.0.0/README.rst
--rw-r--r--   0        0        0     3140 2023-06-17 22:27:32.227857 pywemo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2889 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/README.md
--rw-r--r--   0        0        0     1254 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/__init__.py
--rw-r--r--   0        0        0     2762 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/color.py
--rw-r--r--   0        0        0     6709 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/discovery.py
--rw-r--r--   0        0        0     2753 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/exceptions.py
--rw-r--r--   0        0        0     1468 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/LICENSE
--rw-r--r--   0        0        0    26370 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/__init__.py
--rw-r--r--   0        0        0       23 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/__init__.py
--rw-r--r--   0        0        0     4843 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/attributes.py
--rw-r--r--   0        0        0     6733 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/db_orm.py
--rw-r--r--   0        0        0     6059 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/long_press.py
--rw-r--r--   0        0        0    14976 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/rules_db.py
--rw-r--r--   0        0        0    12705 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/service.py
--rw-r--r--   0        0        0      912 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.py
--rw-r--r--   0        0        0     6838 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.pyi
--rw-r--r--   0        0        0       60 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/__init__.py
--rw-r--r--   0        0        0   126828 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.py
--rw-r--r--   0        0        0     4305 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.xsd
--rw-r--r--   0        0        0   122520 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.py
--rw-r--r--   0        0        0     3526 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.xsd
--rw-r--r--   0        0        0     7275 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd_types.py
--rw-r--r--   0        0        0    18975 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/bridge.py
--rw-r--r--   0        0        0     2833 2023-06-17 22:27:32.227857 pywemo-1.0.0/pywemo/ouimeaux_device/coffeemaker.py
--rw-r--r--   0        0        0     4826 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/crockpot.py
--rw-r--r--   0        0        0     2250 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/dimmer.py
--rw-r--r--   0        0        0     6433 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/humidifier.py
--rw-r--r--   0        0        0     6125 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/insight.py
--rw-r--r--   0        0        0      328 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/lightswitch.py
--rw-r--r--   0        0        0     1645 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/maker.py
--rw-r--r--   0        0        0      141 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/motion.py
--rw-r--r--   0        0        0      157 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/outdoor_plug.py
--rw-r--r--   0        0        0     1023 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ouimeaux_device/switch.py
--rw-r--r--   0        0        0        0 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/py.typed
--rw-r--r--   0        0        0    11845 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/ssdp.py
--rw-r--r--   0        0        0    28195 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/subscribe.py
--rw-r--r--   0        0        0     4417 2023-06-17 22:27:32.231857 pywemo-1.0.0/pywemo/util.py
--rw-r--r--   0        0        0     8382 1970-01-01 00:00:00.000000 pywemo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-07-03 15:47:34.389949 pywemo-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8322 2023-07-03 15:47:34.389949 pywemo-1.1.0/README.rst
+-rw-r--r--   0        0        0     3196 2023-07-03 15:47:34.389949 pywemo-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2889 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/README.md
+-rw-r--r--   0        0        0     1254 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/__init__.py
+-rw-r--r--   0        0        0     2762 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/color.py
+-rw-r--r--   0        0        0     6709 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/discovery.py
+-rw-r--r--   0        0        0     2753 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/exceptions.py
+-rw-r--r--   0        0        0     1468 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/LICENSE
+-rw-r--r--   0        0        0    26370 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/__init__.py
+-rw-r--r--   0        0        0       23 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/__init__.py
+-rw-r--r--   0        0        0     4843 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/attributes.py
+-rw-r--r--   0        0        0     6733 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/db_orm.py
+-rw-r--r--   0        0        0     6059 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/long_press.py
+-rw-r--r--   0        0        0    14976 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/rules_db.py
+-rw-r--r--   0        0        0    12705 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/service.py
+-rw-r--r--   0        0        0      912 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.py
+-rw-r--r--   0        0        0     6838 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.pyi
+-rw-r--r--   0        0        0       60 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/__init__.py
+-rw-r--r--   0        0        0   126828 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.py
+-rw-r--r--   0        0        0     4305 2023-07-03 15:47:34.389949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.xsd
+-rw-r--r--   0        0        0   122520 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.py
+-rw-r--r--   0        0        0     3526 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.xsd
+-rw-r--r--   0        0        0     7275 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd_types.py
+-rw-r--r--   0        0        0    18975 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/bridge.py
+-rw-r--r--   0        0        0     3345 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/coffeemaker.py
+-rw-r--r--   0        0        0     5035 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/crockpot.py
+-rw-r--r--   0        0        0     2250 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/dimmer.py
+-rw-r--r--   0        0        0     7162 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/humidifier.py
+-rw-r--r--   0        0        0     6125 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/insight.py
+-rw-r--r--   0        0        0      328 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/lightswitch.py
+-rw-r--r--   0        0        0     1645 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/maker.py
+-rw-r--r--   0        0        0      141 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/motion.py
+-rw-r--r--   0        0        0      157 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/outdoor_plug.py
+-rw-r--r--   0        0        0     1023 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ouimeaux_device/switch.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/py.typed
+-rw-r--r--   0        0        0    12531 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/ssdp.py
+-rw-r--r--   0        0        0    28315 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/subscribe.py
+-rw-r--r--   0        0        0     4417 2023-07-03 15:47:34.393949 pywemo-1.1.0/pywemo/util.py
+-rw-r--r--   0        0        0     9084 1970-01-01 00:00:00.000000 pywemo-1.1.0/PKG-INFO
```

### Comparing `pywemo-1.0.0/LICENSE` & `pywemo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/README.rst` & `pywemo-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge| |Docs Badge|
-========================================================================================
+pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge| |Docs Badge| |Scorecard Badge| |Best Practices Badge| |SLSA 3 Badge|
+================================================================================================================================================
 Python 3 module to setup, discover and control WeMo devices.
 
 Dependencies
 ------------
 pyWeMo depends on Python packages: requests, ifaddr, lxml, urllib3
 
 How to use
@@ -153,7 +153,16 @@
     :alt: Coveralls coverage
 .. |PyPI Downloads Badge| image:: https://img.shields.io/pypi/dm/pywemo
     :target: https://pypi.org/project/pywemo/
     :alt: Number of PyPI downloads
 .. |Docs Badge| image:: https://github.com/pywemo/pywemo/actions/workflows/docs.yml/badge.svg
     :target: https://pywemo.github.io/pywemo/
     :alt: API Documentation
+.. |Scorecard Badge| image:: https://api.securityscorecards.dev/projects/github.com/pywemo/pywemo/badge
+    :target: https://securityscorecards.dev/viewer/?uri=github.com/pywemo/pywemo
+    :alt: OpenSSF Scorecard
+.. |Best Practices Badge| image:: https://bestpractices.coreinfrastructure.org/projects/7467/badge
+    :target: https://bestpractices.coreinfrastructure.org/projects/7467
+    :alt: OpenSSF Best Practices
+.. |SLSA 3 Badge| image:: https://slsa.dev/images/gh-badge-level3.svg
+    :target: https://github.com/pywemo/pywemo/releases/latest#user-content-SLSA
+    :alt: SLSA level 3
```

### Comparing `pywemo-1.0.0/pyproject.toml` & `pywemo-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pywemo"
-version = "1.0.0"
+version = "1.1.0"
 description = "Lightweight Python module to discover and control WeMo devices"
 authors = ["Eric Severance <pywemo@esev.com>"]
 license = "MIT"
 
 readme = 'README.rst'
 
 repository = "https://github.com/pywemo/pywemo"
@@ -42,18 +42,18 @@
 pytest-vcr = "1.0.2"
 types-requests = ">=2.0"
 coverage = "^7.2.4"
 hypothesis = "^6.75.3"
 # version of generateDS used to create device.py and service.py in .../api/xsd
 generateDS = "2.41.5"
 # other
-deptry = "^0.11.0"
+deptry = ">=0.11,<0.13"
 pre-commit = ">=2.10,<4.0"
 # docs
-pdoc = "^13.1.1"
+pdoc = ">=13.1.1,<15.0.0"
 
 [tool.poetry.group.bootstrap.dependencies]
 poetry = ">=1.2.0"
 
 [tool.coverage]
   [tool.coverage.run]
   branch = true
@@ -65,16 +65,18 @@
     "*/xsd/service.py",
   ]
   [tool.coverage.lcov]
   output = ".cache/coverage.lcov"
 
 [tool.deptry]
 extend_exclude = ["scripts"]
-ignore_missing = [
-  # These are created by generateDS.
+
+[tool.deptry.per_rule_ignores]
+DEP001 = [
+  # Ignore missing dependencies created by generateDS.
   "StringIO",
   "generatedsnamespaces",
   "generatedscollector",
   "generatedssuper",
   "generatedssupersuper"
 ]
```

### Comparing `pywemo-1.0.0/pywemo/README.md` & `pywemo-1.1.0/pywemo/README.md`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/__init__.py` & `pywemo-1.1.0/pywemo/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/color.py` & `pywemo-1.1.0/pywemo/color.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/discovery.py` & `pywemo-1.1.0/pywemo/discovery.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/exceptions.py` & `pywemo-1.1.0/pywemo/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/LICENSE` & `pywemo-1.1.0/pywemo/ouimeaux_device/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/__init__.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/attributes.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/attributes.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/db_orm.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/db_orm.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/long_press.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/long_press.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/rules_db.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/rules_db.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/service.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/service.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/wemo_services.pyi` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/wemo_services.pyi`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/device.xsd` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/device.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd/service.xsd` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd/service.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/api/xsd_types.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/api/xsd_types.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/bridge.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/bridge.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/coffeemaker.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/coffeemaker.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,40 +13,49 @@
 # CoffeeMaker.deviceevent.GetAttributeList() service call
 # Thus these names/values were not chosen randomly
 # and the numbers have meaning.
 class CoffeeMakerMode(IntEnum):
     """Enum to map WeMo modes to human-readable strings."""
 
     _UNKNOWN = _UNKNOWN
-    # pylint: disable=invalid-name
-    Refill = 0  # reservoir empty and carafe not in place
-    PlaceCarafe = 1  # reservoir has water but carafe not present
-    RefillWater = 2  # carafe present but reservoir is empty
-    Ready = 3
-    Brewing = 4
-    Brewed = 5
-    CleaningBrewing = 6
-    CleaningSoaking = 7
-    BrewFailCarafeRemoved = 8
+    # Note: The UpperMixedCase (invalid) names are deprecated.
+    REFILL = 0  # reservoir empty and carafe not in place
+    Refill = 0  # pylint: disable=invalid-name
+    PLACE_CARAFE = 1  # reservoir has water but carafe not present
+    PlaceCarafe = 1  # pylint: disable=invalid-name
+    REFILL_WATER = 2  # carafe present but reservoir is empty
+    RefillWater = 2  # pylint: disable=invalid-name
+    READY = 3
+    Ready = 3  # pylint: disable=invalid-name
+    BREWING = 4
+    Brewing = 4  # pylint: disable=invalid-name
+    BREWED = 5
+    Brewed = 5  # pylint: disable=invalid-name
+    CLEANING_BREWING = 6
+    CleaningBrewing = 6  # pylint: disable=invalid-name
+    CLEANING_SOAKING = 7
+    CleaningSoaking = 7  # pylint: disable=invalid-name
+    BREW_FAILED_CARAFE_REMOVED = 8
+    BrewFailCarafeRemoved = 8  # pylint: disable=invalid-name
 
     @classmethod
     def _missing_(cls, value: Any) -> CoffeeMakerMode:
         return cls._UNKNOWN
 
 
 MODE_NAMES = {
-    CoffeeMakerMode.Refill: "Refill",
-    CoffeeMakerMode.PlaceCarafe: "PlaceCarafe",
-    CoffeeMakerMode.RefillWater: "RefillWater",
-    CoffeeMakerMode.Ready: "Ready",
-    CoffeeMakerMode.Brewing: "Brewing",
-    CoffeeMakerMode.Brewed: "Brewed",
-    CoffeeMakerMode.CleaningBrewing: "CleaningBrewing",
-    CoffeeMakerMode.CleaningSoaking: "CleaningSoaking",
-    CoffeeMakerMode.BrewFailCarafeRemoved: "BrewFailCarafeRemoved",
+    CoffeeMakerMode.REFILL: "Refill",
+    CoffeeMakerMode.PLACE_CARAFE: "PlaceCarafe",
+    CoffeeMakerMode.REFILL_WATER: "RefillWater",
+    CoffeeMakerMode.READY: "Ready",
+    CoffeeMakerMode.BREWING: "Brewing",
+    CoffeeMakerMode.BREWED: "Brewed",
+    CoffeeMakerMode.CLEANING_BREWING: "CleaningBrewing",
+    CoffeeMakerMode.CLEANING_SOAKING: "CleaningSoaking",
+    CoffeeMakerMode.BREW_FAILED_CARAFE_REMOVED: "BrewFailCarafeRemoved",
 }
 
 
 class _Attributes(TypedDict, total=False):
     Mode: int
 
 
@@ -67,17 +76,17 @@
         return MODE_NAMES.get(self.mode, "Unknown")
 
     def get_state(self, force_update: bool = False) -> int:
         """Return 0 if off and 1 if on."""
         # The base implementation using GetBinaryState doesn't work for
         # CoffeeMaker (always returns 0), so use mode instead.
         # Consider the Coffee Maker to be "on" if it's currently brewing.
-        return int(super().get_state(force_update) == CoffeeMakerMode.Brewing)
+        return int(super().get_state(force_update) == CoffeeMakerMode.BREWING)
 
     def set_state(self, state: int) -> None:
         """Set the state of this device to on or off."""
         # CoffeeMaker cannot be turned off remotely, so ignore the request if
         # state is "falsey"
         if state:
             # Coffee Maker always responds with an error if SetBinaryState is
             # called. Use SetAttributes to change the Mode to "Brewing"
-            self._set_attributes(("Mode", CoffeeMakerMode.Brewing))
+            self._set_attributes(("Mode", CoffeeMakerMode.BREWING))
```

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/crockpot.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/crockpot.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,30 +16,34 @@
 # These enums were derived from the CrockPot.basicevent.GetCrockpotState()
 # service call. Thus these names/values were not chosen randomly and the
 # numbers have meaning.
 class CrockPotMode(IntEnum):
     """Modes for the CrockPot."""
 
     _UNKNOWN = _UNKNOWN
-    # pylint: disable=invalid-name
-    Off = 0
-    Warm = 50
-    Low = 51
-    High = 52
+    # Note: The UpperMixedCase (invalid) names are deprecated.
+    OFF = 0
+    Off = 0  # pylint: disable=invalid-name
+    WARM = 50
+    Warm = 50  # pylint: disable=invalid-name
+    LOW = 51
+    Low = 51  # pylint: disable=invalid-name
+    HIGH = 52
+    High = 52  # pylint: disable=invalid-name
 
     @classmethod
     def _missing_(cls, value: Any) -> CrockPotMode:
         return cls._UNKNOWN
 
 
 MODE_NAMES = {
-    CrockPotMode.Off: "Turned Off",
-    CrockPotMode.Warm: "Warm",
-    CrockPotMode.Low: "Low",
-    CrockPotMode.High: "High",
+    CrockPotMode.OFF: "Turned Off",
+    CrockPotMode.WARM: "Warm",
+    CrockPotMode.LOW: "Low",
+    CrockPotMode.HIGH: "High",
 }
 
 
 class _Attributes(TypedDict, total=False):
     """CrockPot state dictionary type."""
 
     cookedTime: int
@@ -129,22 +133,22 @@
     def get_state(self, force_update: bool = False) -> int:
         """Return 0 if off and 1 if on."""
         # The base implementation using GetBinaryState doesn't work for
         # CrockPot (always returns 0) so use mode instead.
         if force_update or self._attributes.get("mode") is None:
             self.update_attributes()
 
-        return int(self.mode != CrockPotMode.Off)
+        return int(self.mode != CrockPotMode.OFF)
 
     def set_state(self, state: int) -> None:
         """Set the state of this device to on or off."""
         if state:
-            self.update_settings(CrockPotMode.High, self.remaining_time)
+            self.update_settings(CrockPotMode.HIGH, self.remaining_time)
         else:
-            self.update_settings(CrockPotMode.Off, 0)
+            self.update_settings(CrockPotMode.OFF, 0)
 
     def update_settings(self, mode: CrockPotMode, time: int) -> None:
         """Update mode and cooking time."""
         if CrockPotMode(mode) == _UNKNOWN:
             raise ValueError(f"Unknown CrockPotMode: {mode}")
         self.basicevent.SetCrockpotState(mode=str(int(mode)), time=str(time))
```

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/dimmer.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/dimmer.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/humidifier.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/humidifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,75 +11,89 @@
 
 # These enums were derived from Humidifier.deviceevent.GetAttributeList() and
 # thus the names/values were not chosen randomly and the numbers have meaning.
 class FanMode(IntEnum):
     """Enum to map WeMo FanModes to human-readable strings."""
 
     _UNKNOWN = _UNKNOWN
-    # pylint: disable=invalid-name
-    Off = 0  # Fan and device turned off
-    Minimum = 1
-    Low = 2
-    Medium = 3
-    High = 4
-    Maximum = 5
+    # Note: The UpperMixedCase (invalid) names are deprecated.
+    OFF = 0  # Fan and device turned off
+    Off = 0  # pylint: disable=invalid-name
+    MINIMUM = 1
+    Minimum = 1  # pylint: disable=invalid-name
+    LOW = 3
+    Low = 2  # pylint: disable=invalid-name
+    MEDIUM = 3
+    Medium = 3  # pylint: disable=invalid-name
+    HIGH = 4
+    High = 4  # pylint: disable=invalid-name
+    MAXIMUM = 5
+    Maximum = 5  # pylint: disable=invalid-name
 
     @classmethod
     def _missing_(cls, value: Any) -> FanMode:
         return cls._UNKNOWN
 
 
 FAN_MODE_NAMES = {
-    FanMode.Off: "Off",
-    FanMode.Minimum: "Minimum",
-    FanMode.Low: "Low",
-    FanMode.Medium: "Medium",
-    FanMode.High: "High",
-    FanMode.Maximum: "Maximum",
+    FanMode.OFF: "Off",
+    FanMode.MINIMUM: "Minimum",
+    FanMode.LOW: "Low",
+    FanMode.MEDIUM: "Medium",
+    FanMode.HIGH: "High",
+    FanMode.MAXIMUM: "Maximum",
 }
 
 
 class DesiredHumidity(IntEnum):
     """Enum to map WeMo DesiredHumidity to human-readable strings."""
 
     _UNKNOWN = _UNKNOWN
-    # pylint: disable=invalid-name
-    FortyFivePercent = 0
-    FiftyPercent = 1
-    FiftyFivePercent = 2
-    SixtyPercent = 3
-    OneHundredPercent = 4  # "Always On" Mode
+    # Note: The UpperMixedCase (invalid) names are deprecated.
+    PERCENT_45 = 0
+    FortyFivePercent = 0  # pylint: disable=invalid-name
+    PERCENT_50 = 1
+    FiftyPercent = 1  # pylint: disable=invalid-name
+    PERCENT_55 = 2
+    FiftyFivePercent = 2  # pylint: disable=invalid-name
+    PERCENT_60 = 3
+    SixtyPercent = 3  # pylint: disable=invalid-name
+    PERCENT_100 = 4  # "Always On" Mode
+    OneHundredPercent = 4  # pylint: disable=invalid-name
 
     @classmethod
     def _missing_(cls, value: Any) -> DesiredHumidity:
         return cls._UNKNOWN
 
 
 DESIRED_HUMIDITY_NAMES = {
-    DesiredHumidity.FortyFivePercent: "45",
-    DesiredHumidity.FiftyPercent: "50",
-    DesiredHumidity.FiftyFivePercent: "55",
-    DesiredHumidity.SixtyPercent: "60",
-    DesiredHumidity.OneHundredPercent: "100",
+    DesiredHumidity.PERCENT_45: "45",
+    DesiredHumidity.PERCENT_50: "50",
+    DesiredHumidity.PERCENT_55: "55",
+    DesiredHumidity.PERCENT_60: "60",
+    DesiredHumidity.PERCENT_100: "100",
 }
 
 
 class WaterLevel(IntEnum):
     """Enum to map WeMo WaterLevel to human-readable strings."""
 
-    # pylint: disable=invalid-name
-    Empty = 0
-    Low = 1
-    Good = 2
+    # Note: The UpperMixedCase (invalid) names are deprecated.
+    EMPTY = 0
+    Empty = 0  # pylint: disable=invalid-name
+    LOW = 1
+    Low = 1  # pylint: disable=invalid-name
+    GOOD = 2
+    Good = 2  # pylint: disable=invalid-name
 
 
 WATER_LEVEL_NAMES = {
-    WaterLevel.Empty: "Empty",
-    WaterLevel.Low: "Low",
-    WaterLevel.Good: "Good",
+    WaterLevel.EMPTY: "Empty",
+    WaterLevel.LOW: "Low",
+    WaterLevel.GOOD: "Good",
 }
 
 FILTER_LIFE_MAX = 60480
 
 
 class _Attributes(TypedDict, total=False):
     FanMode: int
@@ -127,18 +141,18 @@
         """Return the observed relative humidity in percent (float)."""
         return self._attributes.get("CurrentHumidity", 0.0)
 
     @property
     def water_level(self) -> WaterLevel:
         """Return 0 if water level is Empty, 1 if Low, and 2 if Good."""
         if self._attributes.get("NoWater") == 1:
-            return WaterLevel.Empty
+            return WaterLevel.EMPTY
         if self._attributes.get("WaterAdvise") == 1:
-            return WaterLevel.Low
-        return WaterLevel.Good
+            return WaterLevel.LOW
+        return WaterLevel.GOOD
 
     @property
     def water_level_string(self) -> str:
         """Return Empty, Low, or Good depending on the water level."""
         return WATER_LEVEL_NAMES.get(self.water_level, "Unknown")
 
     @property
```

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/insight.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/insight.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/maker.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/maker.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ouimeaux_device/switch.py` & `pywemo-1.1.0/pywemo/ouimeaux_device/switch.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/pywemo/ssdp.py` & `pywemo-1.1.0/pywemo/ssdp.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 from __future__ import annotations
 
 import logging
 import re
 import select
 import socket
 import threading
+import time
+import uuid
 from datetime import datetime, timedelta
+from wsgiref.handlers import format_date_time
 
 from .ouimeaux_device.api.long_press import VIRTUAL_DEVICE_UDN
 from .util import get_callback_address, interface_addresses
 
 DISCOVER_TIMEOUT = 5
 
 LOG = logging.getLogger(__name__)
@@ -21,33 +24,41 @@
 
 MULTICAST_GROUP = "239.255.255.250"
 MULTICAST_PORT = 1900
 
 # Wemo specific urn:
 ST = "urn:Belkin:service:basicevent:1"
 VIRTUAL_DEVICE_USN = f"{VIRTUAL_DEVICE_UDN}::{ST}"
+MAX_AGE = 86400
 
 SSDP_REPLY = f"""HTTP/1.1 200 OK
-CACHE-CONTROL: max-age=86400
+CACHE-CONTROL: max-age={MAX_AGE}
+DATE: %(date)s
 EXT:
-LOCATION: http://%s/setup.xml
+LOCATION: http://%(callback)s/setup.xml
 OPT: "http://schemas.upnp.org/upnp/1/0/"; ns=01
+01-NLS: %(nls)s
+SERVER: Unspecified, UPnP/1.0, Unspecified
+X-User-Agent: pywemo
 ST: {ST}
 USN: {VIRTUAL_DEVICE_USN}
 
 """  # Newline characters at the the end of SSDP_REPLY are intentional.
 SSDP_REPLY = SSDP_REPLY.replace("\n", "\r\n")
 
 SSDP_NOTIFY = f"""NOTIFY * HTTP/1.1
 HOST: {MULTICAST_GROUP}:{MULTICAST_PORT}
-CACHE-CONTROL: max-age=1800
-LOCATION: http://%s/setup.xml
-SERVER: Unspecified, UPnP/1.0, Unspecified
+CACHE-CONTROL: max-age={MAX_AGE}
+LOCATION: http://%(callback)s/setup.xml
+OPT: "http://schemas.upnp.org/upnp/1/0/"; ns=01
+01-NLS: %(nls)s
 NT: {ST}
-NTS: ssdp:alive
+NTS: %(nts)s
+SERVER: Unspecified, UPnP/1.0, Unspecified
+X-User-Agent: pywemo
 USN: {VIRTUAL_DEVICE_USN}
 
 """  # Newline characters at the the end of SSDP_NOTIFY are intentional.
 SSDP_NOTIFY = SSDP_NOTIFY.replace("\n", "\r\n")
 
 EXPECTED_ST_HEADER = ("ST: " + ST).encode("UTF-8")
 EXPECTED_MAN_HEADER = b'MAN: "ssdp:discover"'
@@ -235,25 +246,30 @@
             callback_port: The port for the SubscriptionRegistry HTTP server.
         """
         self.callback_port = callback_port
         self._thread: threading.Thread | None = None
         self._exit = threading.Event()
         self._thread_exception: Exception | None = None
         self._notify_enabled = True  # Only ever set to False in tests.
+        self._nls_uuid = str(uuid.uuid4())
 
-    def send_notify(self) -> None:
+    def send_notify(self, nts: str) -> None:
         """Send a UPnP NOTIFY message containing the virtual device URL."""
         ssdp_target = (MULTICAST_GROUP, MULTICAST_PORT)
         for addr in interface_addresses():  # Send on all interfaces.
-            callback_addr = get_callback_address(addr, self.callback_port)
+            params = {
+                "callback": get_callback_address(addr, self.callback_port),
+                "nls": self._nls_uuid,
+                "nts": nts,
+            }
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             try:
                 sock.bind((addr, 0))
                 sock.sendto(
-                    (SSDP_NOTIFY % callback_addr).encode("UTF-8"), ssdp_target
+                    (SSDP_NOTIFY % params).encode("UTF-8"), ssdp_target
                 )
             except OSError:
                 pass
             finally:
                 sock.close()
 
     def respond_to_discovery(self) -> None:
@@ -281,16 +297,16 @@
             recv_sock.bind((MULTICAST_GROUP, MULTICAST_PORT))
 
             next_notify = datetime.min
             while not self._exit.is_set():
                 # Periodically send NOTIFY messages.
                 now = datetime.now()
                 if now > next_notify and self._notify_enabled:
-                    next_notify = now + timedelta(minutes=2)
-                    self.send_notify()
+                    next_notify = now + timedelta(seconds=(MAX_AGE / 2) - 30)
+                    self.send_notify("ssdp:alive")
 
                 # Check for new discovery requests.
                 if not select.select([recv_sock], [], [], 1)[0]:
                     continue  # Timeout, no data. Loop again and check for exit
                 msg, sock_addr = recv_sock.recvfrom(1024)
                 lines = msg.splitlines()
                 if len(lines) < 3 or not lines[0].startswith(
@@ -298,26 +314,32 @@
                 ):
                     continue
                 if (
                     EXPECTED_ST_HEADER not in lines
                     or EXPECTED_MAN_HEADER not in lines
                 ):
                     continue
-                callback_addr = get_callback_address(
-                    sock_addr[0],
-                    self.callback_port,
-                )
+                params = {
+                    "callback": get_callback_address(
+                        sock_addr[0], self.callback_port
+                    ),
+                    "date": format_date_time(time.time()),
+                    "nls": self._nls_uuid,
+                }
                 try:
                     send_sock.sendto(
-                        (SSDP_REPLY % callback_addr).encode("UTF-8"), sock_addr
+                        (SSDP_REPLY % params).encode("UTF-8"), sock_addr
                     )
                 except OSError as err:
                     LOG.error(
                         "Failed to send SSDP reply to %r: %s", sock_addr, err
                     )
+
+            if self._notify_enabled:
+                self.send_notify("ssdp:byebye")
         except Exception as exp:
             self._thread_exception = exp  # Used in the stop() method.
             raise
         finally:
             recv_sock.close()
             send_sock.close()
```

### Comparing `pywemo-1.0.0/pywemo/subscribe.py` & `pywemo-1.1.0/pywemo/subscribe.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,35 +68,37 @@
 VIRTUAL_SETUP_XML = f"""<?xml version="1.0"?>
 <root xmlns="urn:Belkin:device-1-0">
   <specVersion>
     <major>1</major>
     <minor>0</minor>
   </specVersion>
   <device>
-    <deviceType>urn:Belkin:device:switch:1</deviceType>
+    <deviceType>urn:Belkin:device:controllee:1</deviceType>
     <friendlyName>pywemo virtual device</friendlyName>
     <manufacturer>pywemo</manufacturer>
     <manufacturerURL>https://github.com/pywemo/pywemo</manufacturerURL>
     <modelDescription>pywemo virtual device</modelDescription>
-    <modelName>LightSwitch</modelName>
+    <modelName>Socket</modelName>
     <modelNumber>1.0</modelNumber>
     <hwVersion>v1</hwVersion>
     <modelURL>http://www.belkin.com/plugin/</modelURL>
-    <serialNumber>VirtualDevice</serialNumber>
+    <serialNumber>PyWemoVirtualDevice</serialNumber>
+    <firmwareVersion>WeMo_US_2.00.2769.PVT</firmwareVersion>
     <UDN>{VIRTUAL_DEVICE_UDN}</UDN>
     <binaryState>0</binaryState>
     <serviceList>
       <service>
         <serviceType>urn:Belkin:service:basicevent:1</serviceType>
         <serviceId>urn:Belkin:serviceId:basicevent1</serviceId>
         <controlURL>/upnp/control/basicevent1</controlURL>
         <eventSubURL>/upnp/event/basicevent1</eventSubURL>
         <SCPDURL>/eventservice.xml</SCPDURL>
       </service>
     </serviceList>
+  <presentationURL>/pluginpres.html</presentationURL>
 </device>
 </root>"""
 
 SOAP_ACTION_RESPONSE = {
     '"urn:Belkin:service:basicevent:1#GetBinaryState"': """<s:Envelope
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
   s:encodingStyle="http://schemas.xmlsoap.org/soap/encoding/">
```

### Comparing `pywemo-1.0.0/pywemo/util.py` & `pywemo-1.1.0/pywemo/util.py`

 * *Files identical despite different names*

### Comparing `pywemo-1.0.0/PKG-INFO` & `pywemo-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywemo
-Version: 1.0.0
+Version: 1.1.0
 Summary: Lightweight Python module to discover and control WeMo devices
 Home-page: https://github.com/pywemo/pywemo
 License: MIT
 Keywords: wemo,api
 Author: Eric Severance
 Author-email: pywemo@esev.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -16,16 +16,16 @@
 Requires-Dist: ifaddr (>=0.1.0)
 Requires-Dist: lxml (>=4.6,<5.0)
 Requires-Dist: requests (>=2.0)
 Requires-Dist: urllib3 (>=1.26.0)
 Project-URL: Repository, https://github.com/pywemo/pywemo
 Description-Content-Type: text/x-rst
 
-pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge| |Docs Badge|
-========================================================================================
+pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge| |Docs Badge| |Scorecard Badge| |Best Practices Badge| |SLSA 3 Badge|
+================================================================================================================================================
 Python 3 module to setup, discover and control WeMo devices.
 
 Dependencies
 ------------
 pyWeMo depends on Python packages: requests, ifaddr, lxml, urllib3
 
 How to use
@@ -175,8 +175,17 @@
     :alt: Coveralls coverage
 .. |PyPI Downloads Badge| image:: https://img.shields.io/pypi/dm/pywemo
     :target: https://pypi.org/project/pywemo/
     :alt: Number of PyPI downloads
 .. |Docs Badge| image:: https://github.com/pywemo/pywemo/actions/workflows/docs.yml/badge.svg
     :target: https://pywemo.github.io/pywemo/
     :alt: API Documentation
+.. |Scorecard Badge| image:: https://api.securityscorecards.dev/projects/github.com/pywemo/pywemo/badge
+    :target: https://securityscorecards.dev/viewer/?uri=github.com/pywemo/pywemo
+    :alt: OpenSSF Scorecard
+.. |Best Practices Badge| image:: https://bestpractices.coreinfrastructure.org/projects/7467/badge
+    :target: https://bestpractices.coreinfrastructure.org/projects/7467
+    :alt: OpenSSF Best Practices
+.. |SLSA 3 Badge| image:: https://slsa.dev/images/gh-badge-level3.svg
+    :target: https://github.com/pywemo/pywemo/releases/latest#user-content-SLSA
+    :alt: SLSA level 3
```

