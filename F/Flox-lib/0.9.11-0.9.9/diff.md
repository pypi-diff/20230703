# Comparing `tmp/Flox-lib-0.9.11.tar.gz` & `tmp/Flox-lib-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flox-lib-0.9.11.tar", last modified: Wed Jan 19 10:23:31 2022, max compression
+gzip compressed data, was "Flox-lib-0.9.9.tar", last modified: Wed Jan 19 08:37:30 2022, max compression
```

## Comparing `Flox-lib-0.9.11.tar` & `Flox-lib-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 10:23:31.694521 Flox-lib-0.9.11/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 10:23:31.694521 Flox-lib-0.9.11/Flox_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-01-19 10:23:31.000000 Flox-lib-0.9.11/Flox_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-01-19 10:23:31.000000 Flox-lib-0.9.11/Flox_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-19 10:23:31.000000 Flox-lib-0.9.11/Flox_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-19 10:23:31.000000 Flox-lib-0.9.11/Flox_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-19 10:23:31.000000 Flox-lib-0.9.11/Flox_lib.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-01-19 10:23:31.694521 Flox-lib-0.9.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 10:23:31.694521 Flox-lib-0.9.11/flox/
--rw-r--r--   0 runner    (1001) docker     (121)    13041 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/flox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/flox/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/flox/launcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2717 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/flox/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/flox/version
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-19 10:23:31.698521 Flox-lib-0.9.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-01-19 10:23:23.000000 Flox-lib-0.9.11/setup.py
+drwxrwxrwx   0 garulf    (1000) garulf    (1000)        0 2022-01-19 08:37:30.911957 Flox-lib-0.9.9/
+drwxrwxrwx   0 garulf    (1000) garulf    (1000)        0 2022-01-19 08:37:30.844659 Flox-lib-0.9.9/Flox_lib.egg-info/
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)      291 2022-01-19 08:37:30.000000 Flox-lib-0.9.9/Flox_lib.egg-info/PKG-INFO
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)      255 2022-01-19 08:37:30.000000 Flox-lib-0.9.9/Flox_lib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)        1 2022-01-19 08:37:30.000000 Flox-lib-0.9.9/Flox_lib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)        1 2022-01-19 08:37:30.000000 Flox-lib-0.9.9/Flox_lib.egg-info/not-zip-safe
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)        5 2022-01-19 08:37:30.000000 Flox-lib-0.9.9/Flox_lib.egg-info/top_level.txt
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)     1090 2021-12-11 21:35:00.000000 Flox-lib-0.9.9/LICENSE.txt
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)      291 2022-01-19 08:37:30.910457 Flox-lib-0.9.9/PKG-INFO
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)      820 2021-12-29 08:19:51.000000 Flox-lib-0.9.9/README.md
+drwxrwxrwx   0 garulf    (1000) garulf    (1000)        0 2022-01-19 08:37:30.896957 Flox-lib-0.9.9/flox/
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)    13435 2022-01-19 08:04:45.000000 Flox-lib-0.9.9/flox/__init__.py
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)     2262 2021-12-11 21:35:00.000000 Flox-lib-0.9.9/flox/clipboard.py
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)     3855 2022-01-10 17:41:46.000000 Flox-lib-0.9.9/flox/launcher.py
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)     2814 2022-01-19 08:01:54.000000 Flox-lib-0.9.9/flox/utils.py
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)       38 2022-01-19 08:37:30.912958 Flox-lib-0.9.9/setup.cfg
+-rwxrwxrwx   0 garulf    (1000) garulf    (1000)      357 2022-01-19 08:37:26.000000 Flox-lib-0.9.9/setup.py
```

### Comparing `Flox-lib-0.9.11/LICENSE.txt` & `Flox-lib-0.9.9/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `Flox-lib-0.9.11/README.md` & `Flox-lib-0.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,7 +34,9 @@
             title=data,
             subtitle=data
         )
 
 if __name__ == "__main__":
     YourClass()
 ```
+
+
```

### Comparing `Flox-lib-0.9.11/flox/__init__.py` & `Flox-lib-0.9.9/flox/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,394 +1,394 @@
-import sys
-import os
-import json
-import time
-import webbrowser
-import urllib.parse
-from datetime import date
-import logging
-import logging.handlers
-from pathlib import Path
-from typing import Union
-from functools import wraps
-from tempfile import gettempdir
-
-from .launcher import Launcher
-
-PLUGIN_MANIFEST = 'plugin.json'
-FLOW_API = 'Flow.Launcher'
-WOX_API = 'Wox'
-LOCALAPPDATA = os.getenv('LOCALAPPDATA')
-FILE_PATH = os.path.dirname(os.path.abspath(__file__))
-CWD = os.getcwd()
-APP_DIR = ""
-
-if "UserData" in CWD.split(os.path.sep):
-    idx = int(CWD.split(os.path.sep).index("UserData"))
-    APP_DIR = os.path.sep.join(CWD.split(os.path.sep)[:idx])
-elif "UserData" in FILE_PATH.split(os.path.sep):
-    idx = int(FILE_PATH.split(os.path.sep).index("UserData"))
-    APP_DIR = os.path.sep.join(FILE_PATH.split(os.path.sep)[:idx])
-else:
-    _appdirs = os.listdir(os.path.join(LOCALAPPDATA, "FlowLauncher"))
-    _versions = []
-    for dir in _appdirs:
-        if "app-" in dir:
-            _version = dir.split("app-")[1]
-            _version = tuple(map(int, (_version.split("."))))
-            _versions.append(_version)
-    _version = ".".join(map(str, max(_versions)))
-    _dir = f"app-{_version}"
-    APP_DIR = os.path.join(LOCALAPPDATA, "FlowLauncher", _dir )
-    
-
-APP_ICONS = os.path.join(APP_DIR, "Images")
-ICON_APP = os.path.join(APP_ICONS, 'app.png')
-ICON_APP_ERROR = os.path.join(APP_ICONS, 'app_error.png')
-ICON_BROWSER = os.path.join(APP_ICONS, 'browser.png')
-ICON_CALCULATOR = os.path.join(APP_ICONS, 'calculator.png')
-ICON_CANCEL = os.path.join(APP_ICONS, 'cancel.png')
-ICON_CLOSE = os.path.join(APP_ICONS, 'close.png')
-ICON_CMD = os.path.join(APP_ICONS, 'cmd.png')
-ICON_COLOR = os.path.join(APP_ICONS, 'color.png')
-ICON_CONTROL_PANEL = os.path.join(APP_ICONS, 'ControlPanel.png')
-ICON_COPY = os.path.join(APP_ICONS, 'copy.png')
-ICON_DELETE_FILE_FOLDER = os.path.join(APP_ICONS, 'deletefilefolder.png')
-ICON_DISABLE = os.path.join(APP_ICONS, 'disable.png')
-ICON_DOWN = os.path.join(APP_ICONS, 'down.png')
-ICON_EXE = os.path.join(APP_ICONS, 'exe.png')
-ICON_FILE = os.path.join(APP_ICONS, 'file.png')
-ICON_FIND = os.path.join(APP_ICONS, 'find.png')
-ICON_FOLDER = os.path.join(APP_ICONS, 'folder.png')
-ICON_HISTORY = os.path.join(APP_ICONS, 'history.png')
-ICON_IMAGE = os.path.join(APP_ICONS, 'image.png')
-ICON_LOCK = os.path.join(APP_ICONS, 'lock.png')
-ICON_LOGOFF = os.path.join(APP_ICONS, 'logoff.png')
-ICON_OK = os.path.join(APP_ICONS, 'ok.png')
-ICON_OPEN = os.path.join(APP_ICONS, 'open.png')
-ICON_PICTURES = os.path.join(APP_ICONS, 'pictures.png')
-ICON_PLUGIN = os.path.join(APP_ICONS, 'plugin.png')
-ICON_PROGRAM = os.path.join(APP_ICONS, 'program.png')
-ICON_RECYCLEBIN = os.path.join(APP_ICONS, 'recyclebin.png')
-ICON_RESTART = os.path.join(APP_ICONS, 'restart.png')
-ICON_SEARCH = os.path.join(APP_ICONS, 'search.png')
-ICON_SETTINGS = os.path.join(APP_ICONS, 'settings.png')
-ICON_SHELL = os.path.join(APP_ICONS, 'shell.png')
-ICON_SHUTDOWN = os.path.join(APP_ICONS, 'shutdown.png')
-ICON_SLEEP = os.path.join(APP_ICONS, 'sleep.png')
-ICON_UP = os.path.join(APP_ICONS, 'up.png')
-ICON_UPDATE = os.path.join(APP_ICONS, 'update.png')
-ICON_URL = os.path.join(APP_ICONS, 'url.png')
-ICON_USER = os.path.join(APP_ICONS, 'user.png')
-ICON_WARNING = os.path.join(APP_ICONS, 'warning.png')
-ICON_WEB_SEARCH = os.path.join(APP_ICONS, 'web_search.png')
-ICON_WORK = os.path.join(APP_ICONS, 'work.png')
-
-
-class Flox(Launcher):
-
-    def __init__(self, lib=None):
-        self._start = time.time()
-        self._api = None
-        self._manifest = None
-        self._results = []
-        self._plugindir = None
-        self._appdata = None
-        self.appdir = APP_DIR
-        self._app_settings = None
-        self._user_keywords = None
-        self._appversion = None
-        self._logger = None
-        self.except_results = False
-        self._settings_path = None
-        self._settings = None
-        self.font_family = '/Resources/#Segoe Fluent Icons'
-        if lib:
-            lib_path = os.path.join(self.plugindir, lib)
-            sys.path.append(lib_path)
-        super().__init__(self.api)
-
-    def _query(self, query):
-        try:
-            self.args = query.lower()
-
-            self.query(query)
-
-        except Exception as e:
-            if self.except_results:
-                self._add_except(e)
-            else:
-                raise
-        return self._results
-
-    def _context_menu(self, data):
-        try:
-
-            self.context_menu(data)
-
-        except Exception as e:
-            if self.except_results:
-                self._add_except(e)
-            else:
-                raise
-        return self._results
-
-    def _add_except(self, e):
-        self.add_item(
-            title=e.__class__.__name__,
-            subtitle=str(e),
-            icon=ICON_APP_ERROR,
-            method='github_issue',
-            parameters=[e.__class__.__name__]
-        )
-
-    def github_issue(self, title, log=None):
-        url = self.manifest['Website']
-        if 'github' in url.lower():
-            if log is None:
-                with open(self.applog, 'r') as l:
-                    log = l.readlines()[-50:]
-            error_msg = urllib.parse.quote_plus(''.join(log))
-            issue_body = f"Please+type+any+relevant+information+here%0A%0A%0A%0A%0A%0A%3Cdetails%3E%3Csummary%3EError+Log%3C%2Fsummary%3E%0A%3Cp%3E%0A%0A%60%60%60%0A{error_msg}%0A%60%60%60%0A%3C%2Fp%3E%0A%3C%2Fdetails%3E"
-            url = f"{url}/issues/new?title={title}&body={issue_body}"
-        webbrowser.open(url)
-
-    def add_item(self, title:str, subtitle:str='', icon:str=None, method:Union[str, callable]=None, parameters:list=None, context:list=None, glyph:str=None, score:int=0, **kwargs):
-
-        item = {
-            "Title": str(title),
-            "SubTitle": str(subtitle),
-            "IcoPath": str(icon) or self.icon,
-            "ContextData": context,
-            "Score": score,
-            "JsonRPCAction": {}
-        }
-        auto_complete_text = kwargs.pop("auto_complete_text", None)
-
-        item["AutoCompleteText"] = auto_complete_text or f'{self.user_keyword} {title}'.replace('* ', '')
-        if method:
-            item['JsonRPCAction']['method'] = getattr(method, "__name__", method)
-            item['JsonRPCAction']['parameters'] = parameters or []
-            item['JsonRPCAction']['dontHideAfterAction'] = kwargs.pop("dont_hide", False)
-        if glyph:
-            item['Glyph'] = {}
-            item['Glyph']['Glyph'] = glyph
-            font_family =  kwargs.pop("font_family", self.font_family)
-            if font_family.startswith("#"):
-                font_family = str(Path(self.plugindir).joinpath(font_family))
-            item['Glyph']['FontFamily'] = font_family
-        for kw in kwargs:
-            item[kw] = kwargs[kw]
-        self._results.append(item)
-        return self._results[-1]
-
-    @property
-    def plugindir(self):
-
-        if not self._plugindir:
-            potential_paths = [
-                os.path.abspath(os.getcwd()),
-                os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
-            ]
-
-            for path in potential_paths:
-
-                while True:
-                    if os.path.exists(os.path.join(path, PLUGIN_MANIFEST)):
-                        self._plugindir = path
-                        break
-                    elif os.path.ismount(path):
-                        self._plugindir = os.getcwd()
-                        break
-
-                    path = os.path.dirname(path)
-
-                if self._plugindir:
-                    break
-
-        return self._plugindir
-
-    @property
-    def manifest(self):
-        if not self._manifest:
-            with open(os.path.join(self.plugindir, PLUGIN_MANIFEST), 'r') as f:
-                self._manifest = json.load(f)
-        return self._manifest
-
-    @property
-    def id(self):
-        return self.manifest['ID']
-
-    @property
-    def icon(self):
-        return self.manifest['IcoPath']
-
-    @property
-    def action_keyword(self):
-        return self.manifest['ActionKeyword']
-
-    @property
-    def version(self):
-        return self.manifest['Version']
-
-    @property
-    def appdata(self):
-        if not self._appdata:
-            # Userdata should be up two directories from plugin root
-            self._appdata = os.path.dirname(os.path.dirname(self.plugindir))
-        return self._appdata
-
-    @property
-    def app_settings(self):
-        if not self._app_settings:
-            with open(os.path.join(self.appdata, 'Settings', 'Settings.json'), 'r') as f:
-                self._app_settings = json.load(f)
-        return self._app_settings
-
-    @property
-    def user_keywords(self):
-        if not self._user_keywords:
-            self._user_keywords = self.app_settings['PluginSettings']['Plugins'].get(self.id, {}).get('UserKeywords', [self.action_keyword])
-        return self._user_keywords
-
-    @property
-    def user_keyword(self):
-        return self.user_keywords[0]
-
-    def appicon(self, icon):
-        return os.path.join(self.appdir, 'images', icon + '.png')
-
-    @property
-    def applog(self):
-        today = date.today().strftime('%Y-%m-%d')
-        file = f"{today}.txt"
-        return os.path.join(self.appdata, 'Logs', self.appversion, file)
-
-    
-    @property
-    def appversion(self):
-        if not self._appversion:
-            self._appversion = os.path.basename(self.appdir).replace('app-', '')
-        return self._appversion
-
-    @property
-    def logfile(self):
-        file = f"{self.manifest['Name']}.log"
-        return os.path.join(self.plugindir, file)
-
-    @property
-    def logger(self):
-        if not self._logger:
-            logger = logging.getLogger('')
-            formatter = logging.Formatter(
-                '%(asctime)s %(levelname)s (%(filename)s): %(message)s',
-                datefmt='%H:%M:%S')
-            logfile = logging.handlers.RotatingFileHandler(
-                    self.logfile,
-                    maxBytes=1024 * 1024,
-                    backupCount=1)
-            logfile.setFormatter(formatter)
-            logger.addHandler(logfile)
-            logger.setLevel(logging.WARNING)
-            self._logger = logger
-        return self._logger
-
-    def logger_level(self, level):
-        if level == "info":
-            self.logger.setLevel(logging.INFO)
-        elif level == "debug":
-            self.logger.setLevel(logging.DEBUG)
-        elif level == "warning":
-            self.logger.setLevel(logging.WARNING)
-        elif level == "error":
-            self.logger.setLevel(logging.ERROR)
-        elif level == "critical":
-            self.logger.setLevel(logging.CRITICAL)
-
-    @property
-    def api(self):
-        if not self._api:
-            launcher = os.path.basename(os.path.dirname(self.appdir))
-            if launcher == 'FlowLauncher':
-                self._api = FLOW_API
-            else:
-                self._api = WOX_API
-        return self._api
-
-    @property
-    def name(self):
-        return self.manifest['Name']
-
-    @property
-    def author(self):
-        return self.manifest['Author']
-
-    @property
-    def settings_path(self):
-        if self._settings_path is None:
-            dirname = self.name
-            setting_file = "Settings.json"
-            self._settings_path = os.path.join(self.appdata, 'Settings', 'Plugins', dirname, setting_file)
-        return self._settings_path
-
-    @property
-    def settings(self):
-        if self._settings is None:
-
-            if not os.path.exists(os.path.dirname(self.settings_path)):
-                os.mkdir(os.path.dirname(self.settings_path))
-            self._settings = Settings(self.settings_path)
-        return self._settings
-
-    def browser_open(self, url):
-        webbrowser.open(url)
-
-class Settings(dict):
-
-    def __init__(self, filepath):
-        super(Settings, self).__init__()
-        self._filepath = filepath
-        self._save = True
-        if os.path.exists(self._filepath):
-            self._load()
-        else:
-            data = {}
-            self.update(data)
-            self.save()
-
-        
-    def _load(self):
-        data = {}
-        with open(self._filepath, 'r') as f:
-            try:
-                data.update(json.load(f))
-            except json.decoder.JSONDecodeError:
-                pass
-
-        self._save = False
-        self.update(data)
-        self._save = True
-
-    def save(self):
-        if self._save:
-            data = {}
-            data.update(self)
-            with open(self._filepath, 'w') as f:
-                json.dump(data, f, sort_keys=True, indent=4)
-        return
-    
-    def __setitem__(self, key, value):
-        super(Settings, self).__setitem__(key, value)
-        self.save()
-
-    def __delitem__(self, key):
-        super(Settings, self).__delitem__(key)
-        self.save()
-
-    def update(self, *args, **kwargs):
-        super(Settings, self).update(*args, **kwargs)
-        self.save()
-
-    def setdefault(self, key, value=None):
-        ret = super(Settings, self).setdefault(key, value)
-        self.save()
-        return ret
+import sys
+import os
+import json
+import time
+import webbrowser
+import urllib.parse
+from datetime import date
+import logging
+import logging.handlers
+from pathlib import Path
+from typing import Union
+from functools import wraps
+from tempfile import gettempdir
+
+from .launcher import Launcher
+
+PLUGIN_MANIFEST = 'plugin.json'
+FLOW_API = 'Flow.Launcher'
+WOX_API = 'Wox'
+LOCALAPPDATA = os.getenv('LOCALAPPDATA')
+FILE_PATH = os.path.dirname(os.path.abspath(__file__))
+CWD = os.getcwd()
+APP_DIR = ""
+
+if "UserData" in CWD.split(os.path.sep):
+    idx = int(CWD.split(os.path.sep).index("UserData"))
+    APP_DIR = os.path.sep.join(CWD.split(os.path.sep)[:idx])
+elif "UserData" in FILE_PATH.split(os.path.sep):
+    idx = int(FILE_PATH.split(os.path.sep).index("UserData"))
+    APP_DIR = os.path.sep.join(FILE_PATH.split(os.path.sep)[:idx])
+else:
+    _appdirs = os.listdir(os.path.join(LOCALAPPDATA, "FlowLauncher"))
+    _versions = []
+    for dir in _appdirs:
+        if "app-" in dir:
+            _version = dir.split("app-")[1]
+            _version = tuple(map(int, (_version.split("."))))
+            _versions.append(_version)
+    _version = ".".join(map(str, max(_versions)))
+    _dir = f"app-{_version}"
+    APP_DIR = os.path.join(LOCALAPPDATA, "FlowLauncher", _dir )
+    
+
+APP_ICONS = os.path.join(APP_DIR, "Images")
+ICON_APP = os.path.join(APP_ICONS, 'app.png')
+ICON_APP_ERROR = os.path.join(APP_ICONS, 'app_error.png')
+ICON_BROWSER = os.path.join(APP_ICONS, 'browser.png')
+ICON_CALCULATOR = os.path.join(APP_ICONS, 'calculator.png')
+ICON_CANCEL = os.path.join(APP_ICONS, 'cancel.png')
+ICON_CLOSE = os.path.join(APP_ICONS, 'close.png')
+ICON_CMD = os.path.join(APP_ICONS, 'cmd.png')
+ICON_COLOR = os.path.join(APP_ICONS, 'color.png')
+ICON_CONTROL_PANEL = os.path.join(APP_ICONS, 'ControlPanel.png')
+ICON_COPY = os.path.join(APP_ICONS, 'copy.png')
+ICON_DELETE_FILE_FOLDER = os.path.join(APP_ICONS, 'deletefilefolder.png')
+ICON_DISABLE = os.path.join(APP_ICONS, 'disable.png')
+ICON_DOWN = os.path.join(APP_ICONS, 'down.png')
+ICON_EXE = os.path.join(APP_ICONS, 'exe.png')
+ICON_FILE = os.path.join(APP_ICONS, 'file.png')
+ICON_FIND = os.path.join(APP_ICONS, 'find.png')
+ICON_FOLDER = os.path.join(APP_ICONS, 'folder.png')
+ICON_HISTORY = os.path.join(APP_ICONS, 'history.png')
+ICON_IMAGE = os.path.join(APP_ICONS, 'image.png')
+ICON_LOCK = os.path.join(APP_ICONS, 'lock.png')
+ICON_LOGOFF = os.path.join(APP_ICONS, 'logoff.png')
+ICON_OK = os.path.join(APP_ICONS, 'ok.png')
+ICON_OPEN = os.path.join(APP_ICONS, 'open.png')
+ICON_PICTURES = os.path.join(APP_ICONS, 'pictures.png')
+ICON_PLUGIN = os.path.join(APP_ICONS, 'plugin.png')
+ICON_PROGRAM = os.path.join(APP_ICONS, 'program.png')
+ICON_RECYCLEBIN = os.path.join(APP_ICONS, 'recyclebin.png')
+ICON_RESTART = os.path.join(APP_ICONS, 'restart.png')
+ICON_SEARCH = os.path.join(APP_ICONS, 'search.png')
+ICON_SETTINGS = os.path.join(APP_ICONS, 'settings.png')
+ICON_SHELL = os.path.join(APP_ICONS, 'shell.png')
+ICON_SHUTDOWN = os.path.join(APP_ICONS, 'shutdown.png')
+ICON_SLEEP = os.path.join(APP_ICONS, 'sleep.png')
+ICON_UP = os.path.join(APP_ICONS, 'up.png')
+ICON_UPDATE = os.path.join(APP_ICONS, 'update.png')
+ICON_URL = os.path.join(APP_ICONS, 'url.png')
+ICON_USER = os.path.join(APP_ICONS, 'user.png')
+ICON_WARNING = os.path.join(APP_ICONS, 'warning.png')
+ICON_WEB_SEARCH = os.path.join(APP_ICONS, 'web_search.png')
+ICON_WORK = os.path.join(APP_ICONS, 'work.png')
+
+
+class Flox(Launcher):
+
+    def __init__(self, lib=None):
+        self._start = time.time()
+        self._api = None
+        self._manifest = None
+        self._results = []
+        self._plugindir = None
+        self._appdata = None
+        self.appdir = APP_DIR
+        self._app_settings = None
+        self._user_keywords = None
+        self._appversion = None
+        self._logger = None
+        self.except_results = False
+        self._settings_path = None
+        self._settings = None
+        self.font_family = '/Resources/#Segoe Fluent Icons'
+        if lib:
+            lib_path = os.path.join(self.plugindir, lib)
+            sys.path.append(lib_path)
+        super().__init__(self.api)
+
+    def _query(self, query):
+        try:
+            self.args = query.lower()
+
+            self.query(query)
+
+        except Exception as e:
+            if self.except_results:
+                self._add_except(e)
+            else:
+                raise
+        return self._results
+
+    def _context_menu(self, data):
+        try:
+
+            self.context_menu(data)
+
+        except Exception as e:
+            if self.except_results:
+                self._add_except(e)
+            else:
+                raise
+        return self._results
+
+    def _add_except(self, e):
+        self.add_item(
+            title=e.__class__.__name__,
+            subtitle=str(e),
+            icon=ICON_APP_ERROR,
+            method='github_issue',
+            parameters=[e.__class__.__name__]
+        )
+
+    def github_issue(self, title, log=None):
+        url = self.manifest['Website']
+        if 'github' in url.lower():
+            if log is None:
+                with open(self.applog, 'r') as l:
+                    log = l.readlines()[-50:]
+            error_msg = urllib.parse.quote_plus(''.join(log))
+            issue_body = f"Please+type+any+relevant+information+here%0A%0A%0A%0A%0A%0A%3Cdetails%3E%3Csummary%3EError+Log%3C%2Fsummary%3E%0A%3Cp%3E%0A%0A%60%60%60%0A{error_msg}%0A%60%60%60%0A%3C%2Fp%3E%0A%3C%2Fdetails%3E"
+            url = f"{url}/issues/new?title={title}&body={issue_body}"
+        webbrowser.open(url)
+
+    def add_item(self, title:str, subtitle:str='', icon:str=None, method:Union[str, callable]=None, parameters:list=None, context:list=None, glyph:str=None, score:int=0, **kwargs):
+
+        item = {
+            "Title": str(title),
+            "SubTitle": str(subtitle),
+            "IcoPath": str(icon) or self.icon,
+            "ContextData": context,
+            "Score": score,
+            "JsonRPCAction": {}
+        }
+        auto_complete_text = kwargs.pop("auto_complete_text", None)
+
+        item["AutoCompleteText"] = auto_complete_text or f'{self.user_keyword} {title}'.replace('* ', '')
+        if method:
+            item['JsonRPCAction']['method'] = getattr(method, "__name__", method)
+            item['JsonRPCAction']['parameters'] = parameters or []
+            item['JsonRPCAction']['dontHideAfterAction'] = kwargs.pop("dont_hide", False)
+        if glyph:
+            item['Glyph'] = {}
+            item['Glyph']['Glyph'] = glyph
+            font_family =  kwargs.pop("font_family", self.font_family)
+            if font_family.startswith("#"):
+                font_family = str(Path(self.plugindir).joinpath(font_family))
+            item['Glyph']['FontFamily'] = font_family
+        for kw in kwargs:
+            item[kw] = kwargs[kw]
+        self._results.append(item)
+        return self._results[-1]
+
+    @property
+    def plugindir(self):
+
+        if not self._plugindir:
+            potential_paths = [
+                os.path.abspath(os.getcwd()),
+                os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
+            ]
+
+            for path in potential_paths:
+
+                while True:
+                    if os.path.exists(os.path.join(path, PLUGIN_MANIFEST)):
+                        self._plugindir = path
+                        break
+                    elif os.path.ismount(path):
+                        self._plugindir = os.getcwd()
+                        break
+
+                    path = os.path.dirname(path)
+
+                if self._plugindir:
+                    break
+
+        return self._plugindir
+
+    @property
+    def manifest(self):
+        if not self._manifest:
+            with open(os.path.join(self.plugindir, PLUGIN_MANIFEST), 'r') as f:
+                self._manifest = json.load(f)
+        return self._manifest
+
+    @property
+    def id(self):
+        return self.manifest['ID']
+
+    @property
+    def icon(self):
+        return self.manifest['IcoPath']
+
+    @property
+    def action_keyword(self):
+        return self.manifest['ActionKeyword']
+
+    @property
+    def version(self):
+        return self.manifest['Version']
+
+    @property
+    def appdata(self):
+        if not self._appdata:
+            # Userdata should be up two directories from plugin root
+            self._appdata = os.path.dirname(os.path.dirname(self.plugindir))
+        return self._appdata
+
+    @property
+    def app_settings(self):
+        if not self._app_settings:
+            with open(os.path.join(self.appdata, 'Settings', 'Settings.json'), 'r') as f:
+                self._app_settings = json.load(f)
+        return self._app_settings
+
+    @property
+    def user_keywords(self):
+        if not self._user_keywords:
+            self._user_keywords = self.app_settings['PluginSettings']['Plugins'].get(self.id, {}).get('UserKeywords', [self.action_keyword])
+        return self._user_keywords
+
+    @property
+    def user_keyword(self):
+        return self.user_keywords[0]
+
+    def appicon(self, icon):
+        return os.path.join(self.appdir, 'images', icon + '.png')
+
+    @property
+    def applog(self):
+        today = date.today().strftime('%Y-%m-%d')
+        file = f"{today}.txt"
+        return os.path.join(self.appdata, 'Logs', self.appversion, file)
+
+    
+    @property
+    def appversion(self):
+        if not self._appversion:
+            self._appversion = os.path.basename(self.appdir).replace('app-', '')
+        return self._appversion
+
+    @property
+    def logfile(self):
+        file = f"{self.manifest['Name']}.log"
+        return os.path.join(self.plugindir, file)
+
+    @property
+    def logger(self):
+        if not self._logger:
+            logger = logging.getLogger('')
+            formatter = logging.Formatter(
+                '%(asctime)s %(levelname)s (%(filename)s): %(message)s',
+                datefmt='%H:%M:%S')
+            logfile = logging.handlers.RotatingFileHandler(
+                    self.logfile,
+                    maxBytes=1024 * 1024,
+                    backupCount=1)
+            logfile.setFormatter(formatter)
+            logger.addHandler(logfile)
+            logger.setLevel(logging.WARNING)
+            self._logger = logger
+        return self._logger
+
+    def logger_level(self, level):
+        if level == "info":
+            self.logger.setLevel(logging.INFO)
+        elif level == "debug":
+            self.logger.setLevel(logging.DEBUG)
+        elif level == "warning":
+            self.logger.setLevel(logging.WARNING)
+        elif level == "error":
+            self.logger.setLevel(logging.ERROR)
+        elif level == "critical":
+            self.logger.setLevel(logging.CRITICAL)
+
+    @property
+    def api(self):
+        if not self._api:
+            launcher = os.path.basename(os.path.dirname(self.appdir))
+            if launcher == 'FlowLauncher':
+                self._api = FLOW_API
+            else:
+                self._api = WOX_API
+        return self._api
+
+    @property
+    def name(self):
+        return self.manifest['Name']
+
+    @property
+    def author(self):
+        return self.manifest['Author']
+
+    @property
+    def settings_path(self):
+        if self._settings_path is None:
+            dirname = self.name
+            setting_file = "Settings.json"
+            self._settings_path = os.path.join(self.appdata, 'Settings', 'Plugins', dirname, setting_file)
+        return self._settings_path
+
+    @property
+    def settings(self):
+        if self._settings is None:
+
+            if not os.path.exists(os.path.dirname(self.settings_path)):
+                os.mkdir(os.path.dirname(self.settings_path))
+            self._settings = Settings(self.settings_path)
+        return self._settings
+
+    def browser_open(self, url):
+        webbrowser.open(url)
+
+class Settings(dict):
+
+    def __init__(self, filepath):
+        super(Settings, self).__init__()
+        self._filepath = filepath
+        self._save = True
+        if os.path.exists(self._filepath):
+            self._load()
+        else:
+            data = {}
+            self.update(data)
+            self.save()
+
+        
+    def _load(self):
+        data = {}
+        with open(self._filepath, 'r') as f:
+            try:
+                data.update(json.load(f))
+            except json.decoder.JSONDecodeError:
+                pass
+
+        self._save = False
+        self.update(data)
+        self._save = True
+
+    def save(self):
+        if self._save:
+            data = {}
+            data.update(self)
+            with open(self._filepath, 'w') as f:
+                json.dump(data, f, sort_keys=True, indent=4)
+        return
+    
+    def __setitem__(self, key, value):
+        super(Settings, self).__setitem__(key, value)
+        self.save()
+
+    def __delitem__(self, key):
+        super(Settings, self).__delitem__(key)
+        self.save()
+
+    def update(self, *args, **kwargs):
+        super(Settings, self).update(*args, **kwargs)
+        self.save()
+
+    def setdefault(self, key, value=None):
+        ret = super(Settings, self).setdefault(key, value)
+        self.save()
+        return ret
```

### Comparing `Flox-lib-0.9.11/flox/clipboard.py` & `Flox-lib-0.9.9/flox/clipboard.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import ctypes
-
-from ctypes.wintypes import BOOL, HWND, HANDLE, HGLOBAL, UINT, LPVOID
-from ctypes import c_size_t as SIZE_T
-
-# Credit for code goes to Mark Ransom at https://stackoverflow.com/a/25678113
-
-OpenClipboard = ctypes.windll.user32.OpenClipboard
-OpenClipboard.argtypes = HWND,
-OpenClipboard.restype = BOOL
-EmptyClipboard = ctypes.windll.user32.EmptyClipboard
-EmptyClipboard.restype = BOOL
-GetClipboardData = ctypes.windll.user32.GetClipboardData
-GetClipboardData.argtypes = UINT,
-GetClipboardData.restype = HANDLE
-SetClipboardData = ctypes.windll.user32.SetClipboardData
-SetClipboardData.argtypes = UINT, HANDLE
-SetClipboardData.restype = HANDLE
-CloseClipboard = ctypes.windll.user32.CloseClipboard
-CloseClipboard.restype = BOOL
-CF_UNICODETEXT = 13
-
-GlobalAlloc = ctypes.windll.kernel32.GlobalAlloc
-GlobalAlloc.argtypes = UINT, SIZE_T
-GlobalAlloc.restype = HGLOBAL
-GlobalLock = ctypes.windll.kernel32.GlobalLock
-GlobalLock.argtypes = HGLOBAL,
-GlobalLock.restype = LPVOID
-GlobalUnlock = ctypes.windll.kernel32.GlobalUnlock
-GlobalUnlock.argtypes = HGLOBAL,
-GlobalSize = ctypes.windll.kernel32.GlobalSize
-GlobalSize.argtypes = HGLOBAL,
-GlobalSize.restype = SIZE_T
-
-GMEM_MOVEABLE = 0x0002
-GMEM_ZEROINIT = 0x0040
-
-unicode_type = type(u'')
-
-class Clipboard(object):
-
-    def get(self):
-        text = None
-        OpenClipboard(None)
-        handle = GetClipboardData(CF_UNICODETEXT)
-        pcontents = GlobalLock(handle)
-        size = GlobalSize(handle)
-        if pcontents and size:
-            raw_data = ctypes.create_string_buffer(size)
-            ctypes.memmove(raw_data, pcontents, size)
-            text = raw_data.raw.decode('utf-16le').rstrip(u'\0')
-        GlobalUnlock(handle)
-        CloseClipboard()
-        return text
-
-    def put(self, s):
-        if not isinstance(s, unicode_type):
-            s = s.decode('mbcs')
-        data = s.encode('utf-16le')
-        OpenClipboard(None)
-        EmptyClipboard()
-        handle = GlobalAlloc(GMEM_MOVEABLE | GMEM_ZEROINIT, len(data) + 2)
-        pcontents = GlobalLock(handle)
-        ctypes.memmove(pcontents, data, len(data))
-        GlobalUnlock(handle)
-        SetClipboardData(CF_UNICODETEXT, handle)
+import ctypes
+
+from ctypes.wintypes import BOOL, HWND, HANDLE, HGLOBAL, UINT, LPVOID
+from ctypes import c_size_t as SIZE_T
+
+# Credit for code goes to Mark Ransom at https://stackoverflow.com/a/25678113
+
+OpenClipboard = ctypes.windll.user32.OpenClipboard
+OpenClipboard.argtypes = HWND,
+OpenClipboard.restype = BOOL
+EmptyClipboard = ctypes.windll.user32.EmptyClipboard
+EmptyClipboard.restype = BOOL
+GetClipboardData = ctypes.windll.user32.GetClipboardData
+GetClipboardData.argtypes = UINT,
+GetClipboardData.restype = HANDLE
+SetClipboardData = ctypes.windll.user32.SetClipboardData
+SetClipboardData.argtypes = UINT, HANDLE
+SetClipboardData.restype = HANDLE
+CloseClipboard = ctypes.windll.user32.CloseClipboard
+CloseClipboard.restype = BOOL
+CF_UNICODETEXT = 13
+
+GlobalAlloc = ctypes.windll.kernel32.GlobalAlloc
+GlobalAlloc.argtypes = UINT, SIZE_T
+GlobalAlloc.restype = HGLOBAL
+GlobalLock = ctypes.windll.kernel32.GlobalLock
+GlobalLock.argtypes = HGLOBAL,
+GlobalLock.restype = LPVOID
+GlobalUnlock = ctypes.windll.kernel32.GlobalUnlock
+GlobalUnlock.argtypes = HGLOBAL,
+GlobalSize = ctypes.windll.kernel32.GlobalSize
+GlobalSize.argtypes = HGLOBAL,
+GlobalSize.restype = SIZE_T
+
+GMEM_MOVEABLE = 0x0002
+GMEM_ZEROINIT = 0x0040
+
+unicode_type = type(u'')
+
+class Clipboard(object):
+
+    def get(self):
+        text = None
+        OpenClipboard(None)
+        handle = GetClipboardData(CF_UNICODETEXT)
+        pcontents = GlobalLock(handle)
+        size = GlobalSize(handle)
+        if pcontents and size:
+            raw_data = ctypes.create_string_buffer(size)
+            ctypes.memmove(raw_data, pcontents, size)
+            text = raw_data.raw.decode('utf-16le').rstrip(u'\0')
+        GlobalUnlock(handle)
+        CloseClipboard()
+        return text
+
+    def put(self, s):
+        if not isinstance(s, unicode_type):
+            s = s.decode('mbcs')
+        data = s.encode('utf-16le')
+        OpenClipboard(None)
+        EmptyClipboard()
+        handle = GlobalAlloc(GMEM_MOVEABLE | GMEM_ZEROINIT, len(data) + 2)
+        pcontents = GlobalLock(handle)
+        ctypes.memmove(pcontents, data, len(data))
+        GlobalUnlock(handle)
+        SetClipboardData(CF_UNICODETEXT, handle)
         CloseClipboard()
```

### Comparing `Flox-lib-0.9.11/flox/utils.py` & `Flox-lib-0.9.9/flox/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-from tempfile import gettempdir
-from urllib import request
-from pathlib import Path
-from functools import wraps
-import json
-from time import time
-import socket
-from concurrent.futures import ThreadPoolExecutor
-import logging
-
-logging = logging.getLogger(__name__)
-
-URL_SCHEMA = [
-    'http://',
-    'https://',
-]
-socket.setdefaulttimeout(15)
-
-def cache(file_name:str, max_age=30, dir=gettempdir()):
-    """
-    Cache decorator
-    """
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            cache_file = Path(dir, file_name)
-            if not cache_file.exists() or time() - cache_file.stat().st_mtime > max_age or cache_file.stat().st_size == 0:
-                data = func(*args, **kwargs)
-                if len(data) != 0 and data is not None:
-                    with open(cache_file, 'w') as f:
-                        json.dump(data, f)
-                return data
-            else:
-                with open(cache_file, 'r') as f:
-                    return json.load(f)
-        return wrapper
-    return decorator
-
-def refresh_cache(file_name:str, dir:str=gettempdir()):
-    """
-    Touch cache file
-    """
-    cache_file = Path(dir, file_name)
-    if cache_file.exists():
-        cache_file.touch()
-
-def cache_path(file_name:str, dir:str=gettempdir()):
-    """
-    Return path to cache file
-    """
-    return Path(dir, file_name)
-
-def remove_cache(file_name:str, dir:str=gettempdir()):
-    """
-    Remove cache file
-    """
-    cache_file = Path(dir, file_name)
-    if cache_file.exists():
-        cache_file.unlink()
-
-def download_file(url:str, path, **kwargs):
-    """
-    Download file from url and save it to dir
-
-    Args:
-        url (str): image url.
-        dir (str): directory to save image.
-        file_name (str): file name to save image.
-
-    Keyword Args:
-        force_download (bool): Force download image even if it exists.
-    """
-    force_download = kwargs.pop('force_download', False)
-    if not force_download and path.exists():
-        return
-    request.urlretrieve(url, path)
-    return Path(path)
-
-def get_icon(url:str, path, file_name:str=None, **kwargs):
-    for schema in URL_SCHEMA:
-        if url.startswith(schema):
-            break
-    else:
-        return url
-    executor = kwargs.pop('executor', False)
-    if file_name is None:
-        file_name = url.split('/')[-1]
-    if not Path(path).is_absolute():
-        path = Path(gettempdir(), path)
-    if not path.exists():
-        path.mkdir()
-    full_path = Path(path, file_name)
-    if not full_path.exists():
-        if executor is False:
-            download_file(url, full_path)
-        else:
-            executor.submit(download_file, url, full_path)
+from tempfile import gettempdir
+from urllib import request
+from pathlib import Path
+from functools import wraps
+import json
+from time import time
+import socket
+from concurrent.futures import ThreadPoolExecutor
+import logging
+
+logging = logging.getLogger(__name__)
+
+URL_SCHEMA = [
+    'http://',
+    'https://',
+]
+socket.setdefaulttimeout(15)
+
+def cache(file_name:str, max_age=30, dir=gettempdir()):
+    """
+    Cache decorator
+    """
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            cache_file = Path(dir, file_name)
+            if not cache_file.exists() or time() - cache_file.stat().st_mtime > max_age or cache_file.stat().st_size == 0:
+                data = func(*args, **kwargs)
+                if len(data) != 0 and data is not None:
+                    with open(cache_file, 'w') as f:
+                        json.dump(data, f)
+                return data
+            else:
+                with open(cache_file, 'r') as f:
+                    return json.load(f)
+        return wrapper
+    return decorator
+
+def refresh_cache(file_name:str, dir:str=gettempdir()):
+    """
+    Touch cache file
+    """
+    cache_file = Path(dir, file_name)
+    if cache_file.exists():
+        cache_file.touch()
+
+def cache_path(file_name:str, dir:str=gettempdir()):
+    """
+    Return path to cache file
+    """
+    return Path(dir, file_name)
+
+def remove_cache(file_name:str, dir:str=gettempdir()):
+    """
+    Remove cache file
+    """
+    cache_file = Path(dir, file_name)
+    if cache_file.exists():
+        cache_file.unlink()
+
+def download_file(url:str, path, **kwargs):
+    """
+    Download file from url and save it to dir
+
+    Args:
+        url (str): image url.
+        dir (str): directory to save image.
+        file_name (str): file name to save image.
+
+    Keyword Args:
+        force_download (bool): Force download image even if it exists.
+    """
+    force_download = kwargs.pop('force_download', False)
+    if not force_download and path.exists():
+        return
+    request.urlretrieve(url, path)
+    return Path(path)
+
+def get_icon(url:str, path, file_name:str=None, **kwargs):
+    for schema in URL_SCHEMA:
+        if url.startswith(schema):
+            break
+    else:
+        return url
+    executor = kwargs.pop('executor', False)
+    if file_name is None:
+        file_name = url.split('/')[-1]
+    if not Path(path).is_absolute():
+        path = Path(gettempdir(), path)
+    if not path.exists():
+        path.mkdir()
+    full_path = Path(path, file_name)
+    if not full_path.exists():
+        if executor is False:
+            download_file(url, full_path)
+        else:
+            executor.submit(download_file, url, full_path)
     return full_path
```

