# Comparing `tmp/pyowletapi-2023.5.9.tar.gz` & `tmp/pyowletapi-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyowletapi-2023.5.9.tar", last modified: Tue May  9 08:52:39 2023, max compression
+gzip compressed data, was "pyowletapi-2023.7.1.tar", last modified: Mon Jul  3 13:35:46 2023, max compression
```

## Comparing `pyowletapi-2023.5.9.tar` & `pyowletapi-2023.7.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.392864 pyowletapi-2023.5.9/
--rw-rw-rw-   0        0        0     2326 2023-05-09 08:52:39.393864 pyowletapi-2023.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     1496 2023-05-09 08:51:20.000000 pyowletapi-2023.5.9/README.md
--rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.5.9/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-09 08:52:39.396865 pyowletapi-2023.5.9/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-09 08:42:29.000000 pyowletapi-2023.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.335864 pyowletapi-2023.5.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.357884 pyowletapi-2023.5.9/src/pyowletapi/
--rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.5.9/src/pyowletapi/__init__.py
--rw-rw-rw-   0        0        0    10605 2023-05-09 08:45:32.000000 pyowletapi-2023.5.9/src/pyowletapi/api.py
--rw-rw-rw-   0        0        0      318 2023-05-03 10:36:51.000000 pyowletapi-2023.5.9/src/pyowletapi/exceptions.py
--rw-rw-rw-   0        0        0     4306 2023-05-09 08:46:26.000000 pyowletapi-2023.5.9/src/pyowletapi/owlet.py
--rw-rw-rw-   0        0        0     7398 2023-05-09 08:45:43.000000 pyowletapi-2023.5.9/src/pyowletapi/sock.py
-drwxrwxrwx   0        0        0        0 2023-05-09 08:52:39.390863 pyowletapi-2023.5.9/src/pyowletapi.egg-info/
--rw-rw-rw-   0        0        0     2326 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 08:52:39.000000 pyowletapi-2023.5.9/src/pyowletapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.285499 pyowletapi-2023.7.1/
+-rw-rw-rw-   0        0        0     1869 2023-07-03 13:35:46.286498 pyowletapi-2023.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1496 2023-05-09 08:51:20.000000 pyowletapi-2023.7.1/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-02 10:29:46.000000 pyowletapi-2023.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-07-03 13:35:46.288498 pyowletapi-2023.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      819 2023-07-03 13:35:33.000000 pyowletapi-2023.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.190511 pyowletapi-2023.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.250498 pyowletapi-2023.7.1/src/pyowletapi/
+-rw-rw-rw-   0        0        0       17 2023-05-02 10:29:46.000000 pyowletapi-2023.7.1/src/pyowletapi/__init__.py
+-rw-rw-rw-   0        0        0    18256 2023-05-26 13:48:59.000000 pyowletapi-2023.7.1/src/pyowletapi/api.py
+-rw-rw-rw-   0        0        0     2507 2023-07-03 09:18:19.000000 pyowletapi-2023.7.1/src/pyowletapi/const.py
+-rw-rw-rw-   0        0        0      636 2023-05-26 13:37:20.000000 pyowletapi-2023.7.1/src/pyowletapi/exceptions.py
+-rw-rw-rw-   0        0        0     4306 2023-05-09 08:46:26.000000 pyowletapi-2023.7.1/src/pyowletapi/owlet.py
+-rw-rw-rw-   0        0        0     7388 2023-05-25 15:44:47.000000 pyowletapi-2023.7.1/src/pyowletapi/sock.py
+drwxrwxrwx   0        0        0        0 2023-07-03 13:35:46.283498 pyowletapi-2023.7.1/src/pyowletapi.egg-info/
+-rw-rw-rw-   0        0        0     1869 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 13:35:46.000000 pyowletapi-2023.7.1/src/pyowletapi.egg-info/top_level.txt
```

### Comparing `pyowletapi-2023.5.9/PKG-INFO` & `pyowletapi-2023.7.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.9
+Version: 2023.7.1
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
-License: UNKNOWN
-Description: # Introduction
-        
-        First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
-        
-        inspiration and API reverse engineering taken from various projects:
-        
-        https://github.com/BastianPoe/owlet_api
-        
-        https://github.com/mbevand/owlet_monitor
-        
-        
-        End goal is to create a homeassistant integration using this API. But the intention is that this library will always be usable standalone
-        
-        ## Install
-        To install via pip run command 
-        
-        ```
-        pip install pyowletapi
-        ```
-        
-        ## To do
-        Tidy up exception logging
-        
-        Create test routines
-        
-        ## Use
-        import the api and sock objects
-        
-        ```python
-        from pyowletapi.api import OwletAPI
-        from pyowlet.sock import Sock
-        ```
-        
-        create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
-        
-        ```python
-        api = OwletAPI('europe', username, password)
-        ```
-        
-        you can then authenticate against the Owlet servers using this object and create a list of sock objects
-        
-        ```python
-        await api.authenticate()
-        socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
-        ```
-        
-        to get current reading from sock call the update_properties function on each sock object
-        ```python
-        device.update_properties()
-        ```
-        This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
-        
 Keywords: owlet,api,baby
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+
+# Introduction
+
+First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
+
+inspiration and API reverse engineering taken from various projects:
+
+https://github.com/BastianPoe/owlet_api
+
+https://github.com/mbevand/owlet_monitor
+
+
+End goal is to create a homeassistant integration using this API. But the intention is that this library will always be usable standalone
+
+## Install
+To install via pip run command 
+
+```
+pip install pyowletapi
+```
+
+## To do
+Tidy up exception logging
+
+Create test routines
+
+## Use
+import the api and sock objects
+
+```python
+from pyowletapi.api import OwletAPI
+from pyowlet.sock import Sock
+```
+
+create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
+
+```python
+api = OwletAPI('europe', username, password)
+```
+
+you can then authenticate against the Owlet servers using this object and create a list of sock objects
+
+```python
+await api.authenticate()
+socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
+```
+
+to get current reading from sock call the update_properties function on each sock object
+```python
+device.update_properties()
+```
+This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
```

### Comparing `pyowletapi-2023.5.9/README.md` & `pyowletapi-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.9/setup.py` & `pyowletapi-2023.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
-   
     name="pyowletapi",
-    version="2023.05.9",
+    version="2023.07.01",
     description="Owlet baby montior API wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RyanClark123/pyowletapi",
     author="Ryan Clark",
-    classifiers=[ 
-        "License :: OSI Approved :: MIT License",        
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
     ],
-    
     keywords="owlet, api, baby",
-    package_dir={"": "src"}, 
-    packages=find_packages(where="src"), 
-    python_requires=">=3.9",
-    
-    install_requires=["aiohttp"], 
-)
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
+    python_requires=">=3.10",
+    install_requires=["aiohttp"],
+)
```

### Comparing `pyowletapi-2023.5.9/src/pyowletapi/owlet.py` & `pyowletapi-2023.7.1/src/pyowletapi/owlet.py`

 * *Files identical despite different names*

### Comparing `pyowletapi-2023.5.9/src/pyowletapi/sock.py` & `pyowletapi-2023.7.1/src/pyowletapi/sock.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import logging
 from logging import Logger
 import json
 import datetime
-from .api import OwletAPI
-from typing import Union
+from .api import OwletAPI, TokenDict
+from .const import PROPERTIES, VITALS
+from typing import Union, TypedDict
 
 logger: Logger = logging.getLogger(__package__)
 
-CHARGING_STATUSES = ["NOT CHARGING", "CHARGING", "CHARGED"]
 
+class PropertiesDict(TypedDict):
+    raw_properties: dict
+    properties: dict
+    tokens: Union[None, TokenDict]
 
 class Sock:
     """
     Class representing a Owlet sock device
 
     Attributes
     ----------
@@ -62,29 +66,37 @@
         Constructs an Owlet sock object representing the owlet sock device
 
         Parameters
         ----------
         api (OwletAPI):OwletAPI object used to call the Owlet API
         data (dict):Data returned from the Owlet API showing the details of the sock
         """
+        self._api = api
         self._name = data["product_name"]
         self._model = data["model"]
         self._serial = data["dsn"]
         self._oem_model = data["oem_model"]
         self._sw_version = data["sw_version"]
         self._mac = data["mac"]
         self._lan_ip = data["lan_ip"]
         self._connection_status = data["connection_status"]
         self._device_type = data["device_type"]
         self._manuf_model = data["manuf_model"]
+        self._version = None
 
-        self._api = api
+        self._raw_properties = {}
+        self._properties = {}
 
-        self.raw_properties = {}
-        self.properties = {}
+    @property
+    def api(self) -> OwletAPI:
+        return self._api
+
+    @property
+    def version(self) -> int:
+        return self._version
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def model(self) -> str:
@@ -118,102 +130,101 @@
     def device_type(self) -> str:
         return self._device_type
 
     @property
     def manuf_model(self) -> str:
         return self._manuf_model
 
+    @property
+    def properties(self) -> dict[str:str]:
+        return self._properties
+
+    @property
+    def raw_properties(self) -> dict:
+        return self._raw_properties
+
     def get_property(self, property: str) -> str:
         """
         Returns the specific property based on the property argument passed in
 
         Parameters
         ----------
         property (str):The required property
 
         Returns
         -------
         (str):Request property as a string
         """
-        return self.properties[property]
+        return self._properties[property]
 
-    def get_properties(self) -> dict[str:str]:
-        """
-        Returns all properties for the Owlet sock object
-
-        Returns
-        -------
-        (dict):Request properties as a dict
-        """
-        return self.properties
-
-    async def normalise_properties(
-        self, raw_properties: dict[str:dict]
-    ) -> dict[str : Union[bool, str, float]]:
+    async def normalise_properties(self) -> dict[str : Union[bool, str, float]]:
         """
         Takes the raw properties dictionary returned from the API and formats it into another dict that is more stripped down and easier to work with
 
         Parameters
         ----------
             raw_properties (dict[str:dict]):The raw properties returned from the API call
 
         Returns
         -------
             (dict):Returns the stripped down properties as a dict
         """
         properties = {}
-        properties["app_active"] = bool(raw_properties["APP_ACTIVE"]["value"])
 
-        properties["high_heart_rate_alert"] = bool(
-            raw_properties["HIGH_HR_ALRT"]["value"]
-        )
-        properties["high_oxygen_alert"] = bool(raw_properties["HIGH_OX_ALRT"]["value"])
-        properties["low_battery_alert"] = bool(raw_properties["LOW_BATT_ALRT"]["value"])
-        properties["low_heart_rate_alert"] = bool(
-            raw_properties["LOW_HR_ALRT"]["value"]
-        )
-        properties["low_oxygen_alert"] = bool(raw_properties["LOW_OX_ALRT"]["value"])
-        properties["ppg_log_file"] = bool(raw_properties["PPG_LOG_FILE"]["value"])
-        properties["firmware_update_available"] = bool(
-            raw_properties["FW_UPDATE_STATUS"]["value"]
-        )
-        properties["lost_power_alert"] = bool(
-            raw_properties["LOST_POWER_ALRT"]["value"]
-        )
-        properties["sock_disconnected"] = bool(
-            raw_properties["SOCK_DISCON_ALRT"]["value"]
-        )
-        properties["sock_off"] = bool(raw_properties["SOCK_OFF"]["value"])
-
-        vitals = json.loads(raw_properties["REAL_TIME_VITALS"]["value"])
-        properties["oxygen_saturation"] = float(vitals["ox"])
-        properties["heart_rate"] = float(vitals["hr"])
-        properties["moving"] = bool(vitals["mv"])
-        properties["base_station_on"] = (
-            True if bool(vitals["bso"]) or bool(vitals["chg"]) else False
-        )
-        properties["battery_percentage"] = float(vitals["bat"])
-        properties["battery_minutes"] = float(vitals["btt"])
-        properties["charging"] = True if int(vitals["chg"]) in [1, 2] else False
-        properties["signal_strength"] = float(vitals["rsi"])
-        properties["last_updated"] = datetime.datetime.strptime(
-            raw_properties["REAL_TIME_VITALS"]["data_updated_at"], "%Y-%m-%dT%H:%M:%SZ"
-        ).strftime("%Y/%m/%d %H:%M:%S")
+        for type, properties_tmp in PROPERTIES.items():
+            properties = {
+                key: type(self._raw_properties[property]["value"])
+                for key, property in properties_tmp.items()
+            }
+
+        if self._version == 3:
+            vitals = json.loads(self._raw_properties["REAL_TIME_VITALS"]["value"])
+
+            for type, vitals_tmp in VITALS.items():
+                for key, property in vitals_tmp.items():
+                    match key:
+                        case "base_station_on":
+                            properties[key] = bool(vitals["bso"]) or bool(vitals["chg"])
+                        case "last_updated":
+                            properties[key] = datetime.datetime.strptime(
+                                self._raw_properties["REAL_TIME_VITALS"][
+                                    "data_updated_at"
+                                ],
+                                "%Y-%m-%dT%H:%M:%SZ",
+                            ).strftime("%Y/%m/%d %H:%M:%S")
+                        case _:
+                            properties[key] = type(vitals[property])
 
         return properties
 
+    async def _check_version(self) -> None:
+        version = 0
+        if "REAL_TIME_VITALS" in self._raw_properties:
+            version = 3
+        elif "CHARGE_STATUS" in self._raw_properties:
+            version = 2
+        self._version = version
+
     async def update_properties(
         self,
-    ) -> tuple[dict[str, dict], dict[str : Union[bool, str, float]]]:
+    ) -> PropertiesDict:
         """
-        Calls the Owlet api to update the properties and then returns both the raw response dict and the formatted dict from
-        normalise_properties
+        Calls the Owlet api to update the properties and then returns the raw response dict, the formatted dict from
+        normalise_properties and any new api tokens if they have changed
 
         Returns
         -------
-        (tuple):Tuple containing two dictionaries, one with the raw json response from the API and another with the stripped down properties from normalise_properties
+        (dict):Dictionary containing three dictionaries, one with the raw json response from the API and another with the stripped down
+        properties from normalise_properties, the third will contain the new api tokens if they have changed, if they haven't changed this will be None
         """
         logging.info(f"Updating properties for device {self.serial}")
-        self.raw_properties = await self._api.get_properties(self.serial)
-        self.properties = await self.normalise_properties(self.raw_properties)
-
-        return (self.raw_properties, self.properties)
+        properties = await self._api.get_properties(self.serial)
+        self._raw_properties = properties["response"]
+        if self._version is None:
+            await self._check_version()
+        self._properties = await self.normalise_properties()
+
+        return {
+            "raw_properties": self._raw_properties,
+            "properties": self._properties,
+            "tokens": properties["tokens"],
+        }
```

### Comparing `pyowletapi-2023.5.9/src/pyowletapi.egg-info/PKG-INFO` & `pyowletapi-2023.7.1/src/pyowletapi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 Metadata-Version: 2.1
 Name: pyowletapi
-Version: 2023.5.9
+Version: 2023.7.1
 Summary: Owlet baby montior API wrapper
 Home-page: https://github.com/RyanClark123/pyowletapi
 Author: Ryan Clark
-License: UNKNOWN
-Description: # Introduction
-        
-        First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
-        
-        inspiration and API reverse engineering taken from various projects:
-        
-        https://github.com/BastianPoe/owlet_api
-        
-        https://github.com/mbevand/owlet_monitor
-        
-        
-        End goal is to create a homeassistant integration using this API. But the intention is that this library will always be usable standalone
-        
-        ## Install
-        To install via pip run command 
-        
-        ```
-        pip install pyowletapi
-        ```
-        
-        ## To do
-        Tidy up exception logging
-        
-        Create test routines
-        
-        ## Use
-        import the api and sock objects
-        
-        ```python
-        from pyowletapi.api import OwletAPI
-        from pyowlet.sock import Sock
-        ```
-        
-        create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
-        
-        ```python
-        api = OwletAPI('europe', username, password)
-        ```
-        
-        you can then authenticate against the Owlet servers using this object and create a list of sock objects
-        
-        ```python
-        await api.authenticate()
-        socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
-        ```
-        
-        to get current reading from sock call the update_properties function on each sock object
-        ```python
-        device.update_properties()
-        ```
-        This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
-        
 Keywords: owlet,api,baby
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+
+# Introduction
+
+First pass at creating a wrapper for the Owlet baby monitor api, this currently only supports the sock v3 as I do not have a v2 to test with
+
+inspiration and API reverse engineering taken from various projects:
+
+https://github.com/BastianPoe/owlet_api
+
+https://github.com/mbevand/owlet_monitor
+
+
+End goal is to create a homeassistant integration using this API. But the intention is that this library will always be usable standalone
+
+## Install
+To install via pip run command 
+
+```
+pip install pyowletapi
+```
+
+## To do
+Tidy up exception logging
+
+Create test routines
+
+## Use
+import the api and sock objects
+
+```python
+from pyowletapi.api import OwletAPI
+from pyowlet.sock import Sock
+```
+
+create an api object passing your region, username and password, the OwletAPI will also take a aiohttp session as a keyword argument
+
+```python
+api = OwletAPI('europe', username, password)
+```
+
+you can then authenticate against the Owlet servers using this object and create a list of sock objects
+
+```python
+await api.authenticate()
+socks = {device['device']['dsn']: Sock(api, device['device']) for device in devices}
+```
+
+to get current reading from sock call the update_properties function on each sock object
+```python
+device.update_properties()
+```
+This will return a tuple, the first element being the raw response as a dict and the second element is a more cut down dict version of the response showing only the most relevant data.
```

