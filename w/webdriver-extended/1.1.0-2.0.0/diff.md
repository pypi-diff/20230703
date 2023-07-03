# Comparing `tmp/webdriver-extended-1.1.0.tar.gz` & `tmp/webdriver_extended-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/webdriver-extended-1.1.0.tar", last modified: Sat Nov 14 20:27:59 2020, max compression
+gzip compressed data, was "webdriver_extended-2.0.0.tar", max compression
```

## Comparing `webdriver-extended-1.1.0.tar` & `webdriver_extended-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxrwxr-x   0 zeke      (1000) zeke      (1000)        0 2020-11-14 20:27:59.959648 webdriver-extended-1.1.0/
--rw-rw-r--   0 zeke      (1000) zeke      (1000)      647 2020-11-14 20:27:59.959648 webdriver-extended-1.1.0/PKG-INFO
--rw-rw-r--   0 zeke      (1000) zeke      (1000)      290 2020-11-10 23:52:11.000000 webdriver-extended-1.1.0/README.md
--rw-rw-r--   0 zeke      (1000) zeke      (1000)       38 2020-11-14 20:27:59.959648 webdriver-extended-1.1.0/setup.cfg
--rw-rw-r--   0 zeke      (1000) zeke      (1000)      722 2020-11-10 18:07:37.000000 webdriver-extended-1.1.0/setup.py
-drwxrwxr-x   0 zeke      (1000) zeke      (1000)        0 2020-11-14 20:27:59.959648 webdriver-extended-1.1.0/webdriver_extended/
--rw-rw-r--   0 zeke      (1000) zeke      (1000)       73 2020-11-14 20:27:59.000000 webdriver-extended-1.1.0/webdriver_extended/__init__.py
-drwxrwxr-x   0 zeke      (1000) zeke      (1000)        0 2020-11-14 20:27:59.959648 webdriver-extended-1.1.0/webdriver_extended/chrome/
--rw-rw-r--   0 zeke      (1000) zeke      (1000)        0 2020-11-06 02:06:35.000000 webdriver-extended-1.1.0/webdriver_extended/chrome/__init__.py
--rw-rw-r--   0 zeke      (1000) zeke      (1000)     1514 2020-11-06 02:11:16.000000 webdriver-extended-1.1.0/webdriver_extended/chrome/webdriver.py
--rw-rw-r--   0 zeke      (1000) zeke      (1000)     6545 2020-11-14 20:13:15.000000 webdriver-extended-1.1.0/webdriver_extended/chrome/webelement.py
-drwxrwxr-x   0 zeke      (1000) zeke      (1000)        0 2020-11-14 20:27:59.959648 webdriver-extended-1.1.0/webdriver_extended.egg-info/
--rw-rw-r--   0 zeke      (1000) zeke      (1000)      647 2020-11-14 20:27:59.000000 webdriver-extended-1.1.0/webdriver_extended.egg-info/PKG-INFO
--rw-rw-r--   0 zeke      (1000) zeke      (1000)      375 2020-11-14 20:27:59.000000 webdriver-extended-1.1.0/webdriver_extended.egg-info/SOURCES.txt
--rw-rw-r--   0 zeke      (1000) zeke      (1000)        1 2020-11-14 20:27:59.000000 webdriver-extended-1.1.0/webdriver_extended.egg-info/dependency_links.txt
--rw-rw-r--   0 zeke      (1000) zeke      (1000)       24 2020-11-14 20:27:59.000000 webdriver-extended-1.1.0/webdriver_extended.egg-info/requires.txt
--rw-rw-r--   0 zeke      (1000) zeke      (1000)       19 2020-11-14 20:27:59.000000 webdriver-extended-1.1.0/webdriver_extended.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1068 2023-01-10 02:22:40.000000 webdriver_extended-2.0.0/LICENSE
+-rw-r--r--   0        0        0      290 2023-01-10 02:22:40.000000 webdriver_extended-2.0.0/README.md
+-rw-r--r--   0        0        0      732 2023-01-10 02:23:19.720169 webdriver_extended-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-01-10 02:23:19.722169 webdriver_extended-2.0.0/webdriver_extended/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 02:22:40.000000 webdriver_extended-2.0.0/webdriver_extended/chrome/__init__.py
+-rw-r--r--   0        0        0     1566 2023-01-10 02:22:40.000000 webdriver_extended-2.0.0/webdriver_extended/chrome/webdriver.py
+-rw-r--r--   0        0        0     6549 2023-01-10 02:22:40.000000 webdriver_extended-2.0.0/webdriver_extended/chrome/webelement.py
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 webdriver_extended-2.0.0/setup.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 webdriver_extended-2.0.0/PKG-INFO
```

### Comparing `webdriver-extended-1.1.0/webdriver_extended/chrome/webdriver.py` & `webdriver_extended-2.0.0/webdriver_extended/chrome/webdriver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import os
+import typing
 import uuid
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 
 from .webelement import WebElement
 
 # JavaScript in Python; nice
-IS_HEADLESS_SCRIPT = "return navigator.plugins.length == 0"
+IS_HEADLESS_SCRIPT = "return navigator.plugins.length == 0;"
 
 
 class WebDriver(webdriver.Chrome):
     """webdriver.Chrome, but with more stuff"""
+
     _web_element_cls = WebElement
 
     def __init__(self, *args, **kwargs):
         self.download_dir_name = os.path.abspath(
-            os.path.join(os.sep, "tmp", f".downloads-{uuid.uuid4()}"))
+            os.path.join(os.sep, "tmp", f".downloads-{uuid.uuid4()}")
+        )
         options = kwargs.get("options", Options())
         prefs = options.experimental_options.get("prefs", {})
         prefs.update({"download.default_directory": self.download_dir_name})
         options.add_experimental_option("prefs", prefs)
         kwargs["options"] = options
         super().__init__(*args, **kwargs)
 
     @property
-    def headless(self):
+    def headless(self) -> bool:
         return self.execute_script(IS_HEADLESS_SCRIPT)
 
-    def new_tab(self, url=None, switch_to=True):
+    def new_tab(self, url: typing.Optional[str] = None, switch_to: bool = True):
         """Open a new tab
 
         Args:
             url (str, optional): The URL. If None, open a blank tab. Defaults to None.
             switch_to (bool, optional): If True, switch to the new tab. Defaults to True.
         """
-        if url is None:
-            url = ""
         original_window = self.current_window_handle
         self.execute_script("window.open('');")
         self.switch_to.window(self.window_handles[-1])
-        self.get(url)
+        if url is not None:
+            self.get(url)
         if not switch_to:
             self.switch_to.window(original_window)
```

### Comparing `webdriver-extended-1.1.0/webdriver_extended/chrome/webelement.py` & `webdriver_extended-2.0.0/webdriver_extended/chrome/webelement.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,106 +1,101 @@
 import logging
 import os
 import shutil
+import typing
 from pathlib import Path
 from time import sleep
 
-from selenium import webdriver
 from selenium.common.exceptions import WebDriverException
+from selenium.webdriver.remote.webelement import WebElement
+
+if typing.TYPE_CHECKING:
+    from .webdriver import WebDriver
 
 LOGGER = logging.getLogger(__name__)
 
-GET_FILES_SCRIPT = """a = document.querySelector('downloads-manager').shadowRoot.querySelectorAll('#mainContainer downloads-item');
-b = [];
-for (i = 0; i < a.length; i++) {
-    c = a[i];
-    try {
-        p = c.shadowRoot.querySelector('#progress').value
-    }
-    catch (TypeError) {
-        p = 100
-    }
-    b.push({"file_name" : c.content.querySelector('#file-link').text, "progress" : p});
-}
-return b;"""
+GET_FILES_SCRIPT = """
+let downloads = [];
+document.querySelector('downloads-manager').shadowRoot.querySelectorAll('#mainContainer downloads-item').forEach((download) => {
+    downloads.push({"file_name" : download.data.fileName, "progress" : download.data.percent, "state": download.data.state});
+});
+return downloads;"""
 CLEAR_DOWNLOADS_SCRIPT = "document.querySelector('downloads-manager').shadowRoot.querySelector('#toolbar').shadowRoot.querySelector('#moreActionsMenu').querySelector('button.clear-all').click()"
 
 
-class WebElement(webdriver.remote.webelement.WebElement):
-    def click_to_download(self, max_download_started_check_num=30):
+class WebElement(WebElement):
+    def click_to_download(self, max_download_started_check_num: int = 30):
         """Click on an element to download a file to the current directory
 
         Args:
             max_download_started_check_num (int, optional): Max number of times to check if a download started. Defaults to 30.
 
         Raises:
-        Raises:
             FileNotFoundError: If the file never started downloading
-            NotImplementedError: If you attempt to use this on anything besides ChromeExtended
         """
-        driver = self._parent
+        driver: "WebDriver" = self._parent
         if driver.headless:
             LOGGER.info("Headless, so using click_to_download_2")
             # Use older, more error-prone method, as unfortunately this only loads a blank page if headless
             return self.click_to_download_2()
         original_window = driver.current_window_handle
+        download_dir_name = driver.download_dir_name
         try:
-            download_dir_name = driver.download_dir_name
             Path(download_dir_name).mkdir(parents=True, exist_ok=True)
             # Wait for folder unlock
             while os.path.isfile(os.path.join(download_dir_name, ".lock")):
                 sleep(1)
             # Write lock file
             with open(os.path.join(download_dir_name, ".lock"), "w") as f:
                 f.write("")
             self.click()
             driver.new_tab(url="chrome://downloads")
             # Wait for one download to start
             download_started_check_num = 0
             downloading_files = []
             while not downloading_files:
                 download_started_check_num += 1
-                downloading_files = driver.execute_script(
-                    GET_FILES_SCRIPT)
+                downloading_files = driver.execute_script(GET_FILES_SCRIPT)
                 if not downloading_files:
                     if download_started_check_num == max_download_started_check_num:
-                        raise FileNotFoundError(
-                            "Download never started")
+                        raise FileNotFoundError("Download(s) never started")
                     else:
                         sleep(2)
                 else:
                     break
             # Poll until all downloads are done
-            while True:
-                if all(f["progress"] == 100 for f in downloading_files):
-                    break
-                else:
-                    sleep(1)
+            while not all(f["progress"] == -2 for f in downloading_files):
+                downloading_files = driver.execute_script(GET_FILES_SCRIPT)
+                sleep(1)
             for f in downloading_files:
                 file_name = f["file_name"]
-                shutil.move(os.path.join(
-                    download_dir_name, file_name), file_name)
+                state = f["state"]
+                if state != "COMPLETE":
+                    LOGGER.warning(
+                        f"{file_name} did not complete downloading. State is {state}"
+                    )
+                else:
+                    shutil.move(os.path.join(download_dir_name, file_name), file_name)
             # Clear all
             driver.execute_script(CLEAR_DOWNLOADS_SCRIPT)
         finally:
             driver.switch_to.window(original_window)
             try:
                 shutil.rmtree(download_dir_name)
             except FileNotFoundError:
                 pass
 
-    def click_to_download_2(self, max_download_started_check_num=30):
-        """Click on an element to download a file to the current directory. Uses a worse, more error-prone algorithm
+    def click_to_download_2(self, max_download_started_check_num: int = 30):
+        """Click on an element to download a file to the current directory. Uses a worse, more error-prone algorithm, as it expects only one item to be downloaded on a click
 
         Args:
             max_download_started_check_num (int, optional): Max number of times to check if a download started. Defaults to 30.
 
         Raises:
             FileNotFoundError: If the file never started downloading
-            NotImplementedError: If you attempt to use this on anything besides ChromeExtended
         """
         driver = self._parent
         download_dir_name = driver.download_dir_name
         Path(download_dir_name).mkdir(parents=True, exist_ok=True)
         try:
             # Wait for folder unlock
             while os.path.isfile(os.path.join(download_dir_name, ".lock")):
@@ -115,16 +110,15 @@
                 download_started_check_num = 0
                 while not download_started:
                     download_started_check_num += 1
                     try:
                         if os.listdir(download_dir_name):
                             download_started = True
                         else:
-                            raise FileNotFoundError(
-                                "Download never started")
+                            raise FileNotFoundError("Download never started")
                     except FileNotFoundError as e:
                         if download_started_check_num == max_download_started_check_num:
                             raise e
                         else:
                             sleep(2)
                 # If the download finished
                 files = os.listdir(download_dir_name)
@@ -133,31 +127,31 @@
                     file_name = files[0]
                     if not file_name.endswith(".crdownload"):
                         break
                 except IndexError:
                     # Not there yet
                     pass
                 sleep(1)
-            shutil.move(os.path.join(
-                download_dir_name, file_name), file_name)
+            shutil.move(os.path.join(download_dir_name, file_name), file_name)
         finally:
             try:
                 shutil.rmtree(download_dir_name)
             except FileNotFoundError:
                 pass
 
     def javascript_click(self, soft=False):
         """Use JavaScript to click the element
 
         Args:
             soft (bool, optional): If True, use onmouseup. Defaults to False.
         """
         driver = self.parent
-        driver.execute_script("arguments[0].click();", self) if not soft else driver.execute_script(
-            "arguments[0].onmouseup();", self)
+        driver.execute_script(
+            "arguments[0].click();", self
+        ) if not soft else driver.execute_script("arguments[0].onmouseup();", self)
 
     def bruteforce_click(self):
-        """Try to click the element normally and if causes an exception, use JavaScript instead"""
+        """Try to click the element normally, and if causes an exception, use JavaScript instead"""
         try:
             self.click()
         except WebDriverException:
             self.javascript_click()
```

