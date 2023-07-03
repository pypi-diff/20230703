# Comparing `tmp/selenium_injector-2.1.tar.gz` & `tmp/selenium_injector-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_injector-2.1.tar", last modified: Tue Jun 27 08:06:16 2023, max compression
+gzip compressed data, was "dist\selenium_injector-2.2.tar", last modified: Mon Jul  3 16:13:20 2023, max compression
```

## Comparing `selenium_injector-2.1.tar` & `selenium_injector-2.2.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.1/LICENSE.md
--rw-rw-rw-   0        0        0      228 2023-06-20 11:58:10.000000 selenium_injector-2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5124 2023-06-27 08:06:16.000000 selenium_injector-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3818 2023-06-26 17:27:31.000000 selenium_injector-2.1/README.md
--rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.1/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.1/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-06-27 08:06:16.000000 selenium_injector-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1826 2023-06-20 11:40:08.000000 selenium_injector-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/
--rw-rw-rw-   0        0        0       21 2023-06-27 08:05:47.000000 selenium_injector-2.1/src/selenium_injector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/extension/
--rw-rw-rw-   0        0        0     3032 2023-06-26 17:42:08.000000 selenium_injector-2.1/src/selenium_injector/files/extension/background.js
--rw-rw-rw-   0        0        0     1924 2023-06-15 07:20:05.000000 selenium_injector-2.1/src/selenium_injector/files/extension/manifest.json
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/js/
--rw-rw-rw-   0        0        0     6058 2023-06-27 07:29:06.000000 selenium_injector-2.1/src/selenium_injector/files/js/connection.js
--rw-rw-rw-   0        0        0      310 2023-06-20 10:28:07.000000 selenium_injector-2.1/src/selenium_injector/files/js/utils.js
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/
--rw-rw-rw-   0        0        0     9216 2023-06-27 07:46:04.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/background.js
--rw-rw-rw-   0        0        0     1924 2023-06-27 07:46:04.000000 selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/manifest.json
--rw-rw-rw-   0        0        0     6050 2023-06-17 13:56:27.000000 selenium_injector-2.1/src/selenium_injector/injector.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.1/src/selenium_injector/scripts/__init__.py
--rw-rw-rw-   0        0        0     7438 2023-06-27 07:15:26.000000 selenium_injector-2.1/src/selenium_injector/scripts/injector.py
--rw-rw-rw-   0        0        0     1576 2023-06-20 10:58:22.000000 selenium_injector-2.1/src/selenium_injector/scripts/js.py
--rw-rw-rw-   0        0        0     1742 2023-06-20 11:34:48.000000 selenium_injector-2.1/src/selenium_injector/scripts/socket.py
--rw-rw-rw-   0        0        0     3804 2023-06-20 12:49:54.000000 selenium_injector-2.1/src/selenium_injector/scripts/sync_websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector/utils/
--rw-rw-rw-   0        0        0        0 2023-06-20 13:26:36.000000 selenium_injector-2.1/src/selenium_injector/utils/__init__.py
--rw-rw-rw-   0        0        0     1584 2023-06-20 11:35:20.000000 selenium_injector-2.1/src/selenium_injector/utils/utils.py
--rw-rw-rw-   0        0        0     2040 2023-06-26 16:52:11.000000 selenium_injector-2.1/src/selenium_injector/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/
--rw-rw-rw-   0        0        0     5124 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1013 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-27 08:06:16.000000 selenium_injector-2.1/src/selenium_injector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-2.2/LICENSE.md
+-rw-rw-rw-   0        0        0      275 2023-07-03 15:31:02.000000 selenium_injector-2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6171 2023-07-03 16:13:20.000000 selenium_injector-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4865 2023-07-03 14:55:29.000000 selenium_injector-2.2/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-2.2/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-07-03 16:13:20.000000 selenium_injector-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1835 2023-07-03 16:06:03.000000 selenium_injector-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/
+-rw-rw-rw-   0        0        0       21 2023-07-03 16:05:19.000000 selenium_injector-2.2/src/selenium_injector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/extension/
+-rw-rw-rw-   0        0        0     2158 2023-07-03 08:21:18.000000 selenium_injector-2.2/src/selenium_injector/files/extension/background.js
+-rw-rw-rw-   0        0        0     1661 2023-07-03 15:10:30.000000 selenium_injector-2.2/src/selenium_injector/files/extension/manifest_2.json
+-rw-rw-rw-   0        0        0     1928 2023-07-03 14:10:59.000000 selenium_injector-2.2/src/selenium_injector/files/extension/manifest_3.json
+-rw-rw-rw-   0        0        0      818 2023-07-03 08:21:18.000000 selenium_injector-2.2/src/selenium_injector/files/extension/stay_alive.js
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/js/
+-rw-rw-rw-   0        0        0     8796 2023-07-02 20:13:16.000000 selenium_injector-2.2/src/selenium_injector/files/js/connection.js
+-rw-rw-rw-   0        0        0      310 2023-06-20 10:28:07.000000 selenium_injector-2.2/src/selenium_injector/files/js/utils.js
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv2_extension/
+-rw-rw-rw-   0        0        0    11075 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv2_extension/background.js
+-rw-rw-rw-   0        0        0     1661 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv2_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/
+-rw-rw-rw-   0        0        0    11893 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/background.js
+-rw-rw-rw-   0        0        0     1928 2023-07-03 15:12:26.000000 selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/manifest.json
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-2.2/src/selenium_injector/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11664 2023-07-03 15:41:38.000000 selenium_injector-2.2/src/selenium_injector/scripts/injector.py
+-rw-rw-rw-   0        0        0     2115 2023-07-02 17:58:37.000000 selenium_injector-2.2/src/selenium_injector/scripts/js.py
+-rw-rw-rw-   0        0        0     2080 2023-07-02 18:08:57.000000 selenium_injector-2.2/src/selenium_injector/scripts/socket.py
+-rw-rw-rw-   0        0        0     6753 2023-07-02 19:26:13.000000 selenium_injector-2.2/src/selenium_injector/scripts/sync_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:26:36.000000 selenium_injector-2.2/src/selenium_injector/utils/__init__.py
+-rw-rw-rw-   0        0        0     1586 2023-07-02 17:56:54.000000 selenium_injector-2.2/src/selenium_injector/utils/utils.py
+-rw-rw-rw-   0        0        0     1992 2023-07-03 14:25:42.000000 selenium_injector-2.2/src/selenium_injector/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector.egg-info/
+-rw-rw-rw-   0        0        0     6171 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2023-07-03 16:13:20.000000 selenium_injector-2.2/src/selenium_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-03 16:13:19.000000 selenium_injector-2.2/src/selenium_injector.egg-info/top_level.txt
```

### Comparing `selenium_injector-2.1/LICENSE.md` & `selenium_injector-2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.1/PKG-INFO` & `selenium_injector-2.2/src/selenium_injector.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium_injector
-Version: 2.1
+Name: selenium-injector
+Version: 2.2
 Summary: inject javascript into chrome
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -65,16 +65,16 @@
 driver.get("https://www.wikipedia.org/")
 driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
 
 js = driver.injector.socket.js
 t = js.types
 u = js.utils
 
+prev_url = driver.current_url[:]
 try:
-    prev_url = driver.current_url[:]
     driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
 except TimeoutError as e:
     if driver.current_url != prev_url:
         pass # new page loaded before send_response
     else:
         raise e
 
@@ -92,26 +92,60 @@
 driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
 driver.injector.proxy.clear()
 driver.quit()
 ```
+#### use events
+```python
+from selenium_injector.webdriver import Chrome
+import json
+
+driver = Chrome()
+
+driver.get("chrome://version")
+
+t = driver.injector.socket.js.types
+
+event_id = driver.injector.socket.make_event_id()
+user = driver.injector.any_user
+
+driver.injector.socket.exec(t.list([
+    t.set_event_id(event_id),
+    t.exec(
+        t.path("chrome.webRequest.onCompleted.addListener"),
+        args=[t.event_callback(), t.value({"urls": ["<all_urls>"]})]
+    )
+]), user=user, max_depth=1)
+
+event = driver.injector.socket.event(event_id, user=user)
+for e in event:  # will block forever
+    e = json.loads(e)
+    data = e["result"][0]
+    time = e["t"]
+    print(time + "\n", data['url'])
+
+```
+warning: as `driver.quit()` isn't called in this example, it will leave files in your temp directories
 
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-- [ ] Add MV2 extension
+- [ ] eval within tab scope from extension
+- [x] Add MV2 extension
   - [ ] change headers
-- [ ] add events
-  - [ ] make protocoll use `UUIDS`'s
+- [x] add events
+  - [x] make protocoll use `UUIDS`'s
+  - [ ] allow response to event within scope
+    - using `(...args) => {new event_handler(...args)}`
 - [x] types.eval
   - [ ] for-loops
   - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
   - [x] manage location api leak
   - [ ] proxy per request
@@ -154,7 +188,8 @@
 * [Selenium-Profiles](https://github.com/kaliiiiiiiiii/Selenium-Profiles)
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
 * [PEG-parser](https://github.com/pegjs/pegjs)
 * [make-SV-stayalive](https://stackoverflow.com/a/75082732/20443541)
+* [stringify-obj](https://stackoverflow.com/a/58416333/20443541)
```

### Comparing `selenium_injector-2.1/README.md` & `selenium_injector-2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 driver.get("https://www.wikipedia.org/")
 driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
 
 js = driver.injector.socket.js
 t = js.types
 u = js.utils
 
+prev_url = driver.current_url[:]
 try:
-    prev_url = driver.current_url[:]
     driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
 except TimeoutError as e:
     if driver.current_url != prev_url:
         pass # new page loaded before send_response
     else:
         raise e
 
@@ -62,26 +62,60 @@
 driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
 driver.injector.proxy.clear()
 driver.quit()
 ```
+#### use events
+```python
+from selenium_injector.webdriver import Chrome
+import json
+
+driver = Chrome()
+
+driver.get("chrome://version")
+
+t = driver.injector.socket.js.types
+
+event_id = driver.injector.socket.make_event_id()
+user = driver.injector.any_user
+
+driver.injector.socket.exec(t.list([
+    t.set_event_id(event_id),
+    t.exec(
+        t.path("chrome.webRequest.onCompleted.addListener"),
+        args=[t.event_callback(), t.value({"urls": ["<all_urls>"]})]
+    )
+]), user=user, max_depth=1)
+
+event = driver.injector.socket.event(event_id, user=user)
+for e in event:  # will block forever
+    e = json.loads(e)
+    data = e["result"][0]
+    time = e["t"]
+    print(time + "\n", data['url'])
+
+```
+warning: as `driver.quit()` isn't called in this example, it will leave files in your temp directories
 
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-- [ ] Add MV2 extension
+- [ ] eval within tab scope from extension
+- [x] Add MV2 extension
   - [ ] change headers
-- [ ] add events
-  - [ ] make protocoll use `UUIDS`'s
+- [x] add events
+  - [x] make protocoll use `UUIDS`'s
+  - [ ] allow response to event within scope
+    - using `(...args) => {new event_handler(...args)}`
 - [x] types.eval
   - [ ] for-loops
   - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
   - [x] manage location api leak
   - [ ] proxy per request
@@ -124,7 +158,8 @@
 * [Selenium-Profiles](https://github.com/kaliiiiiiiiii/Selenium-Profiles)
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
 * [PEG-parser](https://github.com/pegjs/pegjs)
 * [make-SV-stayalive](https://stackoverflow.com/a/75082732/20443541)
+* [stringify-obj](https://stackoverflow.com/a/58416333/20443541)
```

### Comparing `selenium_injector-2.1/build_upload.md` & `selenium_injector-2.2/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-2.1/setup.py` & `selenium_injector-2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-requirements = ['selenium', 'requests', "selenium_profiles", "websockets"]
+requirements = ['selenium', 'requests', "selenium_profiles>=2.2.7.2", "websockets"]
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='selenium_injector',
     author='Aurin Aegerter',
```

### Comparing `selenium_injector-2.1/src/selenium_injector/files/extension/background.js` & `selenium_injector-2.2/src/selenium_injector/files/extension/background.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,39 +1,7 @@
-// Forcing service worker to stay alive by sending a "ping" to a port where noone is listening
-// Essentially it prevents SW to fall asleep after the first 30 secs of work.
-
-const INTERNAL_STAYALIVE_PORT = "Whatever_Port_Name_You_Want"
-var alivePort = null;
-StayAlive();
-
-async function StayAlive() {
-    var lastCall = Date.now();
-    var wakeup = setInterval(() => {
-
-        const now = Date.now();
-        const age = now - lastCall;
-
-        if (alivePort == null) {
-            alivePort = chrome.runtime.connect({
-                name: INTERNAL_STAYALIVE_PORT
-            })
-
-            alivePort.onDisconnect.addListener((p) => {
-                alivePort = null;
-            });
-        }
-
-        if (alivePort) {
-            alivePort.postMessage({
-                content: "ping"
-            });
-        }
-    }, 25000);
-}
-
 // chrome extension libs
 
 globalThis.proxy = {}
 proxy.credentials = {}
 
 proxy.set = function(config, patch_webrtc = true, patch_location = true) {
     proxy.config = config
@@ -45,19 +13,18 @@
         webrtc_leak.disable();
     };
     if (patch_location) {
         contentsettings.set_location("block")
     }
 }
 
-proxy.get = function() {
-    connection.not_return = true;
+proxy.get = function(callback) {
     chrome.proxy.settings.get({
         'incognito': false
-    }, connection.send_back.bind(connection));
+    }, callback);
 }
 
 proxy.clear = function(clear_webrtc = true, clear_location = true) {
     chrome.proxy.settings.clear({});
     if (clear_webrtc) {
         webrtc_leak.clear();
     }
```

### Comparing `selenium_injector-2.1/src/selenium_injector/files/extension/manifest.json` & `selenium_injector-2.2/src/selenium_injector/files/extension/manifest_3.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'name'": "'selenium-injector-mv3'"}*

```diff
@@ -8,15 +8,15 @@
         "extension_pages": "script-src 'self' 'wasm-unsafe-eval'; object-src 'self'"
     },
     "description": "executes code passed from selenium",
     "host_permissions": [
         "<all_urls>"
     ],
     "manifest_version": 3,
-    "name": "selenium-injector",
+    "name": "selenium-injector-mv3",
     "permissions": [
         "activeTab",
         "alarms",
         "background",
         "bookmarks",
         "browsingData",
         "certificateProvider",
```

### Comparing `selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/background.js` & `selenium_injector-2.2/src/selenium_injector/files/js/connection.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,211 +1,130 @@
-// Forcing service worker to stay alive by sending a "ping" to a port where noone is listening
-// Essentially it prevents SW to fall asleep after the first 30 secs of work.
-
-const INTERNAL_STAYALIVE_PORT = "Whatever_Port_Name_You_Want"
-var alivePort = null;
-StayAlive();
-
-async function StayAlive() {
-    var lastCall = Date.now();
-    var wakeup = setInterval(() => {
-
-        const now = Date.now();
-        const age = now - lastCall;
-
-        if (alivePort == null) {
-            alivePort = chrome.runtime.connect({
-                name: INTERNAL_STAYALIVE_PORT
-            })
-
-            alivePort.onDisconnect.addListener((p) => {
-                alivePort = null;
-            });
-        }
-
-        if (alivePort) {
-            alivePort.postMessage({
-                content: "ping"
-            });
-        }
-    }, 25000);
-}
-
-// chrome extension libs
-
-globalThis.proxy = {}
-proxy.credentials = {}
-
-proxy.set = function(config, patch_webrtc = true, patch_location = true) {
-    proxy.config = config
-    chrome.proxy.settings.set({
-        value: proxy.config,
-        scope: "regular"
-    }, function() {});
-    if (patch_webrtc) {
-        webrtc_leak.disable();
-    };
-    if (patch_location) {
-        contentsettings.set_location("block")
-    }
-}
-
-proxy.get = function() {
-    connection.not_return = true;
-    chrome.proxy.settings.get({
-        'incognito': false
-    }, connection.send_back.bind(connection));
-}
-
-proxy.clear = function(clear_webrtc = true, clear_location = true) {
-    chrome.proxy.settings.clear({});
-    if (clear_webrtc) {
-        webrtc_leak.clear();
-    }
-    if (clear_location) {
-        contentsettings.set_location("allow")
-    }
-    delete(proxy.config)
-}
-
-
-proxy.set_auth = function(username, password, urls = ["<all_urls>"]) {
-    proxy.credentials = {
-        "password": password,
-        "username": username,
-        "urls": urls
-    };
-
-    proxy.auth_call = function(details) {
-        return {
-            authCredentials: {
-                username: username,
-                password: password
-            }
-        };
-    }
-    chrome.webRequest.onAuthRequired.addListener(
-        proxy.auth_call, {
-            urls: urls
-        },
-        ['blocking']
-    );
-}
-
-proxy.clear_auth = function(urls = ["<all_urls>"]) {
-    proxy.credentials = {};
-    chrome.webRequest.onAuthRequired.removeListener(
-        proxy.auth_call, {
-            urls: urls
-        },
-        ['blocking']);
-    delete(proxy.auth_call)
-}
-
-globalThis.webrtc_leak = {}
-
-webrtc_leak.disable = function(value = "disable_non_proxied_udp") {
-    // https://github.com/aghorler/WebRTC-Leak-Prevent
-    chrome.privacy.network.webRTCIPHandlingPolicy.set({
-        "value": value
-    });
-}
-
-webrtc_leak.clear = function() {
-    webrtc_leak.disable("default")
-}
-
-globalThis.contentsettings = {}
-
-contentsettings.set = function(setting, value, urls = "<all_urls>") {
-    chrome.contentSettings[setting].set({
-        "primaryPattern": urls,
-        "setting": value
-    }, console.log)
-}
-
-contentsettings.set_location = function(setting = "ask", urls = "<all_urls>") {
-    contentsettings.set("location", setting, urls)
-}
-
-
 class DefaultDict {
     constructor(defaultVal) {
         return new Proxy({}, {
             get: (target, name) => name in target ? target[name] : defaultVal
         })
     }
 }
 
-class connector {
-    constructor(host, port, username) {
-        this.connection = {}
-        this.connection.host = host;
-        this.connection.port = port;
-        this.connection.username = username;
-    }
-
-    // structs
-
-    isFunction(functionToCheck) {
-        return functionToCheck && {}.toString.call(functionToCheck) === '[object Function]';
-    }
-
-    // connection to python
+class handler {
+    constructor(connector, request, debug = false) {
 
-    connect() {
-        this.connection.socket = new WebSocket("ws://" + this.connection.host + ":" + parseInt(this.connection.port));
-        this.connection.socket.addEventListener("open", (event) => {
-            this.connection.socket.send(this.connection.username);
-            this.connection.socket.addEventListener("message", (event) => {
-                this.handler(event.data)
-            });
-        });
-        this.connection.socket.addEventListener("error", (event) => {
-            this.connect()
-        });
-        this.connection.socket.addEventListener("close", (event) => {
-            this.connect()
-        });
-    }
+        this.not_return = false
+        this.status = 200
+        this.max_depht = 2
+        this.event_id = undefined
+        this.connector = connector
+        this.debug = debug
+        var error = undefined
+        var result = undefined
+
+        // protocol
+        // fist 32 chars is request_id, rest is message
+        this.req_id = request.slice(0, 32)
+        request = request.slice(32)
+
+        try { // process request
+            var request = JSON.parse(request)
+
+            if (this.debug) {
+                var debug_msg = {}
+                debug_msg[this.req_id] = request
+                console.log("request", debug_msg)
+            };
 
-    send_back(...results) {
-        var response = '{"result":' + this.stringify(results) + ', "status":' + JSON.stringify(this.status) + '}';
-        console.log({
-            "response": JSON.parse(response)
-        });
-        this.connection.socket.send(response)
-    }
+            if (request.hasOwnProperty("not_return")) {
+                this.not_return = request["not_return"]
+            }
+            if (request.hasOwnProperty("max_depth")) {
+                this.max_depth = request["max_depth"]
+            }
 
-    handler(request) {
-        var request = JSON.parse(request);
-        console.log({
-            "request": request
-        })
-        this.not_return = request["not_return"]
-        this.status = 200
-        var e = undefined
-        try {
             var result = this.eval(request)
+
+            if (this.not_return && result && result.catch && this.isFunction(result.catch)) {
+                // handle async errors
+                result.catch((e) => {
+                    result = {
+                        "message": e.message,
+                        "stack": e.stack
+                    };
+                    this.status = "error"
+                })
+            }
         } catch (e) {
+            // handle sync errors
             var result = {
                 "message": e.message,
                 "stack": e.stack
             };
             this.status = "error"
         };
-        if (this.not_return) {
-            if (e) {
-                throw e
+        if (!(this.not_return) || this.status === "error") {
+            this.send_back(result)
+        }
+    }
+    parse(results, status) {
+        var date = new Date()
+        date = date.toLocaleString()
+
+        try {
+            var parsed = '{"result":' + this.stringify(results, 0, this.max_depth) + ', "status":' + JSON.stringify(status) + ',"t":"' + date + '"}'
+        } catch (e) {
+            var parsed = this.parse([{
+                "message": e.message,
+                "stack": e.stack
+            }], "error")
+        }
+        return parsed
+    }
+
+    send_back(...results) {
+        var resp_id = this.req_id
+
+        var response = this.parse(results, this.status)
+
+        if (this.debug) {
+            var debug_msg = {}
+            var type = "response"
+            if (resp_id[0] === "E") {
+                type = "event"
             }
+            debug_msg[resp_id] = JSON.parse(response)
+            console.log(type, debug_msg)
+        };
+
+        // protocol
+        // fist 32 chars is request_id, rest is message
+        response = resp_id + response
+        this.connector.socket.send(response)
+    }
+    event_callback(...results) {
+        this.req_id = this.event_id
+        if (this.event_id && this.event_id[0] === "E") {
+            this.send_back(...results)
         } else {
-            this.send_back(result)
+            throw new TypeError('event_id isn\'t set or doesn\'t start with "E"')
+        }
+    }
+    set_event_id(event_id) {
+        if (event_id[0] === "E") {
+            this.event_id = event_id
+        } else {
+            throw new TypeError('event_id[0] needs to equal "E", but got: ' + event_id)
         }
     }
 
+    // structs
+
+    isFunction(functionToCheck) {
+        return functionToCheck && {}.toString.call(functionToCheck) === '[object Function]';
+    }
+
+    // eval
     eval(type_json) {
         var defaultdict = new DefaultDict(undefined)
         var type_json = Object.assign({}, defaultdict, type_json)
         var type = type_json["type"];
         switch (type) {
             case "type":
                 var result = this.eval(type_json["type_json"]);
@@ -227,14 +146,17 @@
                 break;
             case "dict":
                 var result = this.dict(type_json["dict_list"]);
                 break;
             case "op":
                 var result = this.op(type_json["op"], this.eval(type_json["a"]), this.eval(type_json["b"]));
                 break;
+            case "!":
+                var result = !(this.eval(type_json["obj"]))
+                break;
             case "this":
                 var result = this
                 break;
             default:
                 throw new TypeError("Expected type_json, but got " + this.stringify(type_json));
         }
         return result;
@@ -270,15 +192,15 @@
         };
     }
 
     list(list) {
         var results = [];
         list.forEach(function(item, index) {
             results.push(this.eval(item))
-        });
+        }.bind(this));
         return results
     }
 
     dict(dict_list) {
         var res_dict = {};
         dict_list.forEach(function(item) {
             res_dict[this.eval(item["key"])] = this.eval(item["val"])
@@ -295,76 +217,117 @@
             } else {
                 var result = this.eval(else_statement)
             }
         };
         return result
     }
 
-    stringify(obj) {
-        var result = JSON.stringify(obj, this.replacer.bind(this))
-        return result
-    }
-
-    replacer(key, value) {
-        // Filtering out properties
-        if (this.isFunction(value)) {
-            this.status = "func_to_str"
-            return value.toLocaleString();
-        } else if (value == undefined) {
-            return null
+    stringify(object, depth = 0, max_depth = 2) {
+        const valid = function(value) {
+            // filter out certain values
+            return !(value == undefined || value == null || typeof value == "function" || value === "")
+        }.bind(this)
+
+        // change max_depth to see more levels, for a touch event, 2 is good
+        if (depth > max_depth)
+            return 'Object';
+
+        var obj = undefined
+        if (Array.isArray(object)) {
+            obj = []
+            object.forEach(function(item, index) {
+                if (item instanceof Object) {
+                    item = this.stringify(item, depth + 1, max_depth)
+                }
+                if (valid(item)) {
+                    obj.push(item)
+                }
+            }.bind(this));
         } else {
-            return value
+            obj = {};
+            for (let key in object) {
+                let value = object[key];
+                if (value instanceof globalThis.constructor)
+                    value = globalThis.constructor.name; // handle recursive
+                else if (value instanceof Object)
+                    value = this.stringify(value, depth + 1, max_depth);
+
+                if (valid(value)) {
+                    obj[key] = value;
+                }
+            }
         }
+
+        return depth ? obj : JSON.stringify(obj);
     }
 
     op(op, a, b) {
-        function num(x) {
-            if (typeof x != "number")
-                throw new Error("Expected number but got " + x);
-            return x;
-        }
-
-        function div(x) {
-            if (num(x) == 0)
-                throw new Error("Divide by zero");
-            return x;
-        }
-        var a = this.eval(a)
-        var b = this.eval(b)
         switch (op) {
             case "+":
                 return a + b;
             case "-":
-                return num(a) - num(b);
+                return a - b;
             case "*":
-                return num(a) * num(b);
+                return a * b;
             case "/":
-                return num(a) / div(b);
+                return a / b;
+            case "^":
+                return a ^ b;
             case "%":
-                return num(a) % div(b);
+                return a % b;
+            case "&":
+                return a & b;
             case "&&":
                 return a && b;
             case "||":
                 return a || b;
             case "|":
                 return a | b;
             case "<":
-                return num(a) < num(b);
+                return a < b;
             case ">":
-                return num(a) > num(b);
+                return a > b;
             case "<=":
-                return num(a) <= num(b);
+                return a <= b;
             case ">=":
-                return num(a) >= num(b);
+                return a >= b;
             case "==":
                 return a == b;
             case "===":
                 return a === b;
             case "!=":
                 return a != b;
+            case "=":
+                return a = b;
         }
         throw new Error("Can't apply operator " + op);
     }
+}
+
+class connector {
+    constructor(host, port, username, handler, debug = false) {
+        this.host = host;
+        this.port = port;
+        this.username = username;
+        this.handler = handler
+        this.debug = debug
+        this.connect()
+    }
+
+    // connection to python
+    connect() {
+        this.socket = new WebSocket("ws://" + this.host + ":" + parseInt(this.port));
+        this.socket.addEventListener("open", (event) => {
+            this.socket.send(this.username);
+            this.socket.addEventListener("message", (event) => {
+                var handler = new this.handler(this, event.data, this.debug)
+            });
+        });
+        this.socket.addEventListener("error", (event) => {
+            this.connect()
+        });
+        this.socket.addEventListener("close", (event) => {
+            this.connect()
+        });
+    }
 
-} //end connector class
-var connection = new connector("localhost", 55065, "selenium-injector-mv3")
-connection.connect();
+} //end connector class
```

### Comparing `selenium_injector-2.1/src/selenium_injector/files/tmp/injector_extension/manifest.json` & `selenium_injector-2.2/src/selenium_injector/files/tmp/mv3_extension/manifest.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'name'": "'selenium-injector-mv3'"}*

```diff
@@ -8,15 +8,15 @@
         "extension_pages": "script-src 'self' 'wasm-unsafe-eval'; object-src 'self'"
     },
     "description": "executes code passed from selenium",
     "host_permissions": [
         "<all_urls>"
     ],
     "manifest_version": 3,
-    "name": "selenium-injector",
+    "name": "selenium-injector-mv3",
     "permissions": [
         "activeTab",
         "alarms",
         "background",
         "bookmarks",
         "browsingData",
         "certificateProvider",
```

### Comparing `selenium_injector-2.1/src/selenium_injector/scripts/js.py` & `selenium_injector-2.2/src/selenium_injector/scripts/js.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 class JS:
     def __init__(self):
         self.types = self.types()
         self.utils = self.utils(self.types)
 
     class types:
+        def __init__(self):
+            self.not_return = {"not_return": True}
+
         def path(self, path: str, obj: dict = None):
             return {"type": "path", "path": path, "obj": obj}
 
         def exec(self, func: dict, args: list = None):
             if not args:
                 args = []
             return {"type": "exec", "func": func, "args": args}
 
         def value(self, value):
             return {"type": "val", "val": value}
 
-        def condition(self, condition: dict, do: dict, elsewhise: dict = None):
-            return {"type": "if", "if": condition, "do": do, "else": elsewhise}
+        def condition(self, condition: dict, do: dict, elsewise: dict = None):
+            return {"type": "if", "if": condition, "do": do, "else": elsewise}
 
         # noinspection PyShadowingBuiltins
         def list(self, list: list = None):
             return {"type": "list", "list": list}
 
         def dict(self, dict_list: list = None):
             return {"type": "dict", "dict_list": dict_list}
 
         def operator(self, a: dict, b: dict, operator: str):
             return {"type": "op", "a": a, "b": b, "op": operator}
 
+        def negation(self, obj: dict):
+            return {"type": "!", "obj": obj}
+
+        def this(self):
+            return {"type": "this"}
+
         def send_back(self):
-            return self.path("send_back", obj={"type": "this"})
+            return self.path("send_back", obj=self.this())
+
+        def event_callback(self):
+            return self.path("event_callback", obj=self.this())
+
+        def set_event_id(self, event_id):
+            return self.exec(self.path("set_event_id", obj=self.this()),
+                             args=[self.value(event_id)]
+                             )
 
     class utils:
         def __init__(self, types):
             self.types = types
 
         def find_element_by_xpath(self, xpath: str):
             return self.types.exec(self.types.path("utils.find_element.ByXpath"),
```

### Comparing `selenium_injector-2.1/src/selenium_injector/utils/utils.py` & `selenium_injector-2.2/src/selenium_injector/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+
 import selenium_injector
 import socket
 from contextlib import closing
 
 
 def sel_injector_path():
     return os.path.dirname(selenium_injector.__file__) + "/"
```

### Comparing `selenium_injector-2.1/src/selenium_injector/webdriver.py` & `selenium_injector-2.2/src/selenium_injector/webdriver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from selenium.webdriver import ChromeOptions
-from selenium_injector.scripts.injector import Injector
+from selenium_injector.scripts.injector import Injector, make_config
 from selenium.webdriver import Chrome as BaseDriver
 import warnings
 
 
 class Chrome(BaseDriver):
     # noinspection PyDefaultArgument
     def __init__(self, injector_options={"port": None, "host": None, "temp_dir": None}, base_drivers: tuple = None,
@@ -21,31 +21,28 @@
             pass
         else:
             Chrome.__bases__ = base_drivers
 
         if not injector_options or injector_options is True:
             injector_options = {}
 
-        self.injector = Injector(**injector_options)
+        self.injector = Injector(debug=True, **injector_options)
 
         if "options" not in kwargs.keys():
             kwargs["options"] = ChromeOptions()
-        kwargs["options"].add_argument(f'--load-extension={self.injector.path}')
+
+        kwargs["options"].add_argument(f'--load-extension={",".join(self.injector.paths)}')
 
         super().__init__(**kwargs)
 
         # connection to tab-0
         tab_index = self.window_handles.index(self.current_window_handle).__str__()
         self.injector.tab_user = "tab-" + tab_index
-        config = f"""
-                var connection = new connector("{self.injector.socket.host}", {self.injector.socket.port}, "{self.injector.tab_user}")
-                connection.connect();
-                """
-
+        config = make_config(self.injector.socket.host, self.injector.socket.port, self.injector.tab_user, debug=True)
         from selenium_injector.utils.utils import read
-        utils_js = read("files/js/utils.js")
+        utils_js = read("files/js/utils.js", sel_root=True)
         self.execute_cdp_cmd("Page.addScriptToEvaluateOnNewDocument",
                              {"source": "(function(){%s})()" % (utils_js + self.injector.connection_js + config)})
 
     def quit(self) -> None:
         self.injector.stop()
         super().quit()
```

### Comparing `selenium_injector-2.1/src/selenium_injector.egg-info/PKG-INFO` & `selenium_injector-2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: selenium-injector
-Version: 2.1
+Name: selenium_injector
+Version: 2.2
 Summary: inject javascript into chrome
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -65,16 +65,16 @@
 driver.get("https://www.wikipedia.org/")
 driver.injector.socket.exec_command("utils.find_element.ByXpath", '//*[@id="js-link-box-en"]/strong', user=driver.injector.tab_user)
 
 js = driver.injector.socket.js
 t = js.types
 u = js.utils
 
+prev_url = driver.current_url[:]
 try:
-    prev_url = driver.current_url[:]
     driver.injector.socket.exec(u.click_element(u.find_element_by_xpath('//*[@id="js-link-box-en"]/strong')), user=driver.injector.tab_user, timeout=2)
 except TimeoutError as e:
     if driver.current_url != prev_url:
         pass # new page loaded before send_response
     else:
         raise e
 
@@ -92,26 +92,60 @@
 driver.injector.proxy.set_single(host="example_host.com", port=143, password="password", username="user-1")
 
 driver.get("https://whatismyipaddress.com/")
 
 driver.injector.proxy.clear()
 driver.quit()
 ```
+#### use events
+```python
+from selenium_injector.webdriver import Chrome
+import json
+
+driver = Chrome()
+
+driver.get("chrome://version")
+
+t = driver.injector.socket.js.types
+
+event_id = driver.injector.socket.make_event_id()
+user = driver.injector.any_user
+
+driver.injector.socket.exec(t.list([
+    t.set_event_id(event_id),
+    t.exec(
+        t.path("chrome.webRequest.onCompleted.addListener"),
+        args=[t.event_callback(), t.value({"urls": ["<all_urls>"]})]
+    )
+]), user=user, max_depth=1)
+
+event = driver.injector.socket.event(event_id, user=user)
+for e in event:  # will block forever
+    e = json.loads(e)
+    data = e["result"][0]
+    time = e["t"]
+    print(time + "\n", data['url'])
+
+```
+warning: as `driver.quit()` isn't called in this example, it will leave files in your temp directories
 
 
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-- [ ] Add MV2 extension
+- [ ] eval within tab scope from extension
+- [x] Add MV2 extension
   - [ ] change headers
-- [ ] add events
-  - [ ] make protocoll use `UUIDS`'s
+- [x] add events
+  - [x] make protocoll use `UUIDS`'s
+  - [ ] allow response to event within scope
+    - using `(...args) => {new event_handler(...args)}`
 - [x] types.eval
   - [ ] for-loops
   - [x] async execution
 - [x] authentificaten proxies
   - [x] manage webrtc-leak
   - [x] manage location api leak
   - [ ] proxy per request
@@ -154,7 +188,8 @@
 * [Selenium-Profiles](https://github.com/kaliiiiiiiiii/Selenium-Profiles)
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
 * [PEG-parser](https://github.com/pegjs/pegjs)
 * [make-SV-stayalive](https://stackoverflow.com/a/75082732/20443541)
+* [stringify-obj](https://stackoverflow.com/a/58416333/20443541)
```

### Comparing `selenium_injector-2.1/src/selenium_injector.egg-info/SOURCES.txt` & `selenium_injector-2.2/src/selenium_injector.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 MANIFEST.in
 README.md
 build_upload.md
 pyproject.toml
 setup.cfg
 setup.py
 src/selenium_injector/__init__.py
-src/selenium_injector/injector.py
 src/selenium_injector/webdriver.py
 src/selenium_injector.egg-info/PKG-INFO
 src/selenium_injector.egg-info/SOURCES.txt
 src/selenium_injector.egg-info/dependency_links.txt
 src/selenium_injector.egg-info/requires.txt
 src/selenium_injector.egg-info/top_level.txt
 src/selenium_injector/files/extension/background.js
-src/selenium_injector/files/extension/manifest.json
+src/selenium_injector/files/extension/manifest_2.json
+src/selenium_injector/files/extension/manifest_3.json
+src/selenium_injector/files/extension/stay_alive.js
 src/selenium_injector/files/js/connection.js
 src/selenium_injector/files/js/utils.js
-src/selenium_injector/files/tmp/injector_extension/background.js
-src/selenium_injector/files/tmp/injector_extension/manifest.json
+src/selenium_injector/files/tmp/mv2_extension/background.js
+src/selenium_injector/files/tmp/mv2_extension/manifest.json
+src/selenium_injector/files/tmp/mv3_extension/background.js
+src/selenium_injector/files/tmp/mv3_extension/manifest.json
 src/selenium_injector/scripts/__init__.py
 src/selenium_injector/scripts/injector.py
 src/selenium_injector/scripts/js.py
 src/selenium_injector/scripts/socket.py
 src/selenium_injector/scripts/sync_websocket.py
 src/selenium_injector/utils/__init__.py
 src/selenium_injector/utils/utils.py
```

