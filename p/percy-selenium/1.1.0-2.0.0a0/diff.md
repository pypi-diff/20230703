# Comparing `tmp/percy-selenium-1.1.0.tar.gz` & `tmp/percy-selenium-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-selenium-1.1.0.tar", last modified: Mon Apr 10 08:09:16 2023, max compression
+gzip compressed data, was "percy-selenium-2.0.0a0.tar", last modified: Mon Jul  3 13:57:04 2023, max compression
```

## Comparing `percy-selenium-1.1.0.tar` & `percy-selenium-2.0.0a0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.050206 percy-selenium-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 08:09:16.050206 percy-selenium-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.046206 percy-selenium-1.1.0/percy/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/percy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/percy/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.046206 percy-selenium-1.1.0/percy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 08:09:16.000000 percy-selenium-1.1.0/percy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:09:16.050206 percy-selenium-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:09:16.046206 percy-selenium-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-04-10 08:08:48.000000 percy-selenium-1.1.0/tests/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/percy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 13:57:04.000000 percy-selenium-2.0.0a0/percy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:57:04.629859 percy-selenium-2.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-07-03 13:56:39.000000 percy-selenium-2.0.0a0/tests/test_snapshot.py
```

### Comparing `percy-selenium-1.1.0/LICENSE` & `percy-selenium-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-selenium-1.1.0/PKG-INFO` & `percy-selenium-2.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-selenium
-Version: 1.1.0
+Version: 2.0.0a0
 Summary: Python client for visual testing with Percy
 Home-page: https://github.com/percy/percy-selenium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: selenium percy visual testing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `percy-selenium-1.1.0/README.md` & `percy-selenium-2.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `percy-selenium-1.1.0/percy/snapshot.py` & `percy-selenium-2.0.0a0/percy/snapshot.py`

 * *Files 23% similar despite different names*

```diff
@@ -77,7 +77,44 @@
         response.raise_for_status()
         data = response.json()
 
         if not data['success']: raise Exception(data['error'])
     except Exception as e:
         print(f'{LABEL} Could not take DOM snapshot "{name}"')
         print(f'{LABEL} {e}')
+
+# Take screenshot on driver
+def percy_automate_screenshot(driver, name, options = None, **kwargs):
+    if not is_percy_enabled(): return
+    if options is None:
+        options = {}
+
+    try:
+        ignore_region_elements = get_element_ids(
+            options.get("ignore_region_selenium_elements", [])
+        )
+        options.pop("ignore_region_selenium_elements", None)
+        options["ignore_region_elements"] = ignore_region_elements
+
+        # Post to automateScreenshot endpoint with driver options and other info
+        response = requests.post(f'{PERCY_CLI_API}/percy/automateScreenshot', json={**kwargs, **{
+            'client_info': CLIENT_INFO,
+            'environment_info': ENV_INFO,
+            'sessionId': driver.session_id,
+            'commandExecutorUrl': driver.command_executor._url, # pylint: disable=W0212
+            'capabilities': dict(driver.capabilities),
+            'sessionCapabilites':dict(driver.desired_capabilities),
+            'snapshotName': name,
+            'options': options
+        }}, timeout=60)
+
+        # Handle errors
+        response.raise_for_status()
+        data = response.json()
+
+        if not data['success']: raise Exception(data['error'])
+    except Exception as e:
+        print(f'{LABEL} Could not take Screenshot "{name}"')
+        print(f'{LABEL} {e}')
+
+def get_element_ids(elements):
+    return [element.id for element in elements]
```

### Comparing `percy-selenium-1.1.0/percy_selenium.egg-info/PKG-INFO` & `percy-selenium-2.0.0a0/percy_selenium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-selenium
-Version: 1.1.0
+Version: 2.0.0a0
 Summary: Python client for visual testing with Percy
 Home-page: https://github.com/percy/percy-selenium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: selenium percy visual testing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `percy-selenium-1.1.0/setup.py` & `percy-selenium-2.0.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `percy-selenium-1.1.0/tests/test_snapshot.py` & `percy-selenium-2.0.0a0/tests/test_snapshot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 import unittest
-from unittest.mock import patch
+from unittest.mock import patch, Mock
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from threading import Thread
 
 import httpretty
 import requests
 from selenium.webdriver import Firefox, FirefoxOptions
+from selenium.webdriver.remote.webdriver import WebDriver
+from selenium.webdriver.remote.webelement import WebElement
+from selenium.webdriver.remote.remote_connection import RemoteConnection
 
-from percy import percy_snapshot, percySnapshot
+from percy import percy_snapshot, percySnapshot, percy_screenshot
 import percy.snapshot as local
+from percy.exception import UnsupportedWebDriverException
 LABEL = local.LABEL
 
 # mock a simple webpage to snapshot
 class MockServerRequestHandler(BaseHTTPRequestHandler):
     def do_GET(self):
         self.send_response(200)
         self.send_header('Content-Type', 'text/html')
         self.end_headers()
         self.wfile.write(('Snapshot Me').encode('utf-8'))
     def log_message(self, format, *args):
         return
 
+class CommandExecutorMock():
+    def __init__(self, url):
+        self._url = url
+
+    def dummy_method(self):
+        pass
+
+    def dummy_method1(self):
+        pass
+
 # daemon threads automatically shut down when the main process exits
 mock_server = HTTPServer(('localhost', 8000), MockServerRequestHandler)
 mock_server_thread = Thread(target=mock_server.serve_forever)
 mock_server_thread.daemon = True
 mock_server_thread.start()
 
 # mock helpers
@@ -53,14 +67,20 @@
 
 def mock_snapshot(fail=False):
     httpretty.register_uri(
         httpretty.POST, 'http://localhost:5338/percy/snapshot',
         body=('{ "success": ' + ('true' if not fail else 'false, "error": "test"') + '}'),
         status=(500 if fail else 200))
 
+def mock_screenshot(fail=False):
+    httpretty.register_uri(
+        httpretty.POST, 'http://localhost:5338/percy/automateScreenshot',
+        body=('{ "success": ' + ('true' if not fail else 'false, "error": "test"') + '}'),
+        status=(500 if fail else 200))
+
 class TestPercySnapshot(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         options = FirefoxOptions()
         options.add_argument('-headless')
         cls.driver = Firefox(options=options)
 
@@ -161,14 +181,126 @@
         mock_healthcheck()
         mock_snapshot(fail=True)
 
         with patch('builtins.print') as mock_print:
             percy_snapshot(self.driver, 'Snapshot 1')
 
             mock_print.assert_any_call(f'{LABEL} Could not take DOM snapshot "Snapshot 1"')
+
+class TestPercyScreenshot(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        driver = Mock(spec=WebDriver)
+        driver.session_id = 'Dummy_session_id'
+        driver.capabilities = { 'key': 'value' }
+        driver.desired_capabilities = { 'key': 'value' }
+        driver.command_executor = Mock(spec=RemoteConnection)
+        driver.command_executor._url = 'https://hub-cloud.browserstack.com/wd/hub' # pylint: disable=W0212
+
+        cls.driver = driver
+
+    @classmethod
+    def tearDownClass(cls):
+        cls.driver.quit()
+
+    def setUp(self):
+        # clear the cached value for testing
+        local.is_percy_enabled.cache_clear()
+        self.driver.get('http://localhost:8000')
+        httpretty.enable()
+
+    def tearDown(self):
+        httpretty.disable()
+        httpretty.reset()
+
+    def test_throws_error_when_a_driver_is_not_provided(self):
+        with self.assertRaises(Exception):
+            percy_screenshot()
+
+    def test_throws_error_when_a_name_is_not_provided(self):
+        with self.assertRaises(Exception):
+            percy_screenshot(self.driver)
+
+    def test_disables_screenshot_when_the_healthcheck_fails(self):
+        mock_healthcheck(fail=True)
+
+        with patch('builtins.print') as mock_print:
+            percy_screenshot(self.driver, 'Snapshot 1')
+            percy_screenshot(self.driver, 'Snapshot 2')
+
+            mock_print.assert_called_with(f'{LABEL} Percy is not running, disabling snapshots')
+
+        self.assertEqual(httpretty.last_request().path, '/percy/healthcheck')
+
+    def test_disables_screenshot_when_the_healthcheck_version_is_wrong(self):
+        mock_healthcheck(fail=True, fail_how='wrong-version')
+
+        with patch('builtins.print') as mock_print:
+            percy_screenshot(self.driver, 'Snapshot 1')
+            percy_screenshot(self.driver, 'Snapshot 2')
+
+            mock_print.assert_called_with(f'{LABEL} Unsupported Percy CLI version, 2.0.0')
+
+        self.assertEqual(httpretty.last_request().path, '/percy/healthcheck')
+
+    def test_disables_screenshot_when_the_healthcheck_version_is_missing(self):
+        mock_healthcheck(fail=True, fail_how='no-version')
+
+        with patch('builtins.print') as mock_print:
+            percy_screenshot(self.driver, 'Snapshot 1')
+            percy_screenshot(self.driver, 'Snapshot 2')
+
+            mock_print.assert_called_with(
+                f'{LABEL} You may be using @percy/agent which is no longer supported by this SDK. '
+                'Please uninstall @percy/agent and install @percy/cli instead. '
+                'https://docs.percy.io/docs/migrating-to-percy-cli')
+
+        self.assertEqual(httpretty.last_request().path, '/percy/healthcheck')
+
+    def test_disables_screenshot_when_the_driver_is_not_selenium(self):
+        mock_healthcheck(fail=True, fail_how='no-version')
+        with self.assertRaises(UnsupportedWebDriverException):
+            percy_screenshot("dummy_driver", 'Snapshot 1')
+
+    def test_posts_screenshot_to_the_local_percy_server(self):
+        mock_healthcheck()
+        mock_screenshot()
+
+        element = Mock(spec=WebElement)
+        element.id = 'Dummy_id'
+        percy_screenshot(self.driver, 'Snapshot 1')
+        percy_screenshot(self.driver, 'Snapshot 2', options = { "enable_javascript": True,
+                          "ignore_region_selenium_elements": [element]})
+
+        self.assertEqual(httpretty.last_request().path, '/percy/automateScreenshot')
+
+        s1 = httpretty.latest_requests()[1].parsed_body
+        self.assertEqual(s1['snapshotName'], 'Snapshot 1')
+        self.assertEqual(s1['sessionId'], self.driver.session_id)
+        self.assertEqual(s1['commandExecutorUrl'], self.driver.command_executor._url) # pylint: disable=W0212
+        self.assertEqual(s1['capabilities'], dict(self.driver.capabilities))
+        self.assertEqual(s1['sessionCapabilites'], dict(self.driver.desired_capabilities))
+        self.assertRegex(s1['client_info'], r'percy-selenium-python/\d+')
+        self.assertRegex(s1['environment_info'][0], r'selenium/\d+')
+        self.assertRegex(s1['environment_info'][1], r'python/\d+')
+
+        s2 = httpretty.latest_requests()[2].parsed_body
+        self.assertEqual(s2['snapshotName'], 'Snapshot 2')
+        self.assertEqual(s2['options']['enable_javascript'], True)
+        self.assertEqual(s2['options']['ignore_region_elements'], ['Dummy_id'])
+
+    def test_handles_screenshot_errors(self):
+        mock_healthcheck()
+        mock_screenshot(fail=True)
+
+        with patch('builtins.print') as mock_print:
+            percy_screenshot(self.driver, 'Snapshot 1')
+
+            mock_print.assert_any_call(f'{LABEL} Could not take Screenshot "Snapshot 1"')
+
 def get_percy_test_requests():
     response = requests.get('http://localhost:5338/test/requests', timeout=10)
     data = response.json()
     return data['requests']
 
 class TestPercySnapshotIntegration(unittest.TestCase):
     @classmethod
```

