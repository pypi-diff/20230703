# Comparing `tmp/zm-au-1.2.0.tar.gz` & `tmp/zm_au-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zm-au-1.2.0.tar", max compression
+gzip compressed data, was "zm_au-2.0.0.tar", max compression
```

## Comparing `zm-au-1.2.0.tar` & `zm_au-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2022-02-19 19:52:55.000000 zm-au-1.2.0/LICENSE
--rw-r--r--   0        0        0     2232 2022-02-19 19:52:55.000000 zm-au-1.2.0/README.md
--rw-r--r--   0        0        0      839 2022-02-19 19:53:40.904522 zm-au-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      306 2022-02-19 19:53:40.905522 zm-au-1.2.0/zm_au/__init__.py
--rw-r--r--   0        0        0     2704 2022-02-19 19:52:55.000000 zm-au-1.2.0/zm_au/base_au.py
--rw-r--r--   0        0        0     1951 2022-02-19 19:52:55.000000 zm-au-1.2.0/zm_au/pip_au.py
--rw-r--r--   0        0        0     3013 2022-02-19 19:52:55.000000 zm-au-1.2.0/zm_au/pip_github_au.py
--rw-r--r--   0        0        0     2959 2022-02-19 19:53:40.953288 zm-au-1.2.0/setup.py
--rw-r--r--   0        0        0     2920 2022-02-19 19:53:40.953484 zm-au-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-05 23:14:04.685300 zm_au-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2232 2023-06-05 23:14:04.685451 zm_au-2.0.0/README.md
+-rw-r--r--   0        0        0     1651 2023-07-03 21:30:56.388346 zm_au-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-07-03 21:30:56.389942 zm_au-2.0.0/zm_au/__init__.py
+-rw-r--r--   0        0        0     2674 2023-06-18 17:42:26.886422 zm_au-2.0.0/zm_au/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 23:14:04.686098 zm_au-2.0.0/zm_au/pip/__init__.py
+-rw-r--r--   0        0        0     2030 2023-06-08 23:38:11.887896 zm_au-2.0.0/zm_au/pip/base.py
+-rw-r--r--   0        0        0     3234 2023-06-08 23:40:36.765056 zm_au-2.0.0/zm_au/pip/github.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 zm_au-2.0.0/PKG-INFO
```

### Comparing `zm-au-1.2.0/LICENSE` & `zm_au-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Zeke Marffy
+Copyright (c) 2023 Zeke Marffy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `zm-au-1.2.0/README.md` & `zm_au-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `zm-au-1.2.0/zm_au/base_au.py` & `zm_au-2.0.0/zm_au/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,82 @@
-import os
 import sys
+from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Union
 
 import packaging.version
 import zmtools
 
 
 class UpdateException(Exception):
     # Base exception class for this module
     pass
 
 
-class BaseAU():
-
-    """Base auto-updater class. Will not work as is; its purpose is to be inherited from
+class BaseAU:
+    """Base auto-updater. Should be inherited from.
 
     Attributes:
-        current_version (str): The current version of the package
-        latest_version (str): The latest version of the package
-        needs_update (bool): If the package is not the latest version
+        current_version (str): The current version of the package.
+        latest_version (str): The latest version of the package.
+        needs_update (bool): If the package is not the latest version.
     """
 
     def __init__(self) -> None:
         self.current_version = self._get_current_version()
         self.latest_version = self._get_latest_version()
 
-    def _get_current_version(self) -> str:
+    def _get_current_version(self) -> str:  # type: ignore
         # Override me!
         # This function must return the current version of the package
         pass
 
-    def _get_latest_version(self) -> str:
+    def _get_latest_version(self) -> str:  # type: ignore
         # Override me!
         # This function must return the latest version of the package
         pass
 
-    def _download(self) -> Union[os.PathLike, str]:
+    def _download(self) -> Path:  # type: ignore
         # Override me!
-        # This function must download the package and return the filename of the downloaded file
+        # This function must download the package and return the path of the downloaded file
         pass
 
-    def _update(self, update_file: Union[os.PathLike, str]) -> None:
+    def _update(self, update_file: Path) -> None:
         # Override me!
         # This function must install a package whose location is passed via the sole parameter
         pass
 
     def update(self, prompt: bool = True) -> None:
-        """Update the package
+        """Update the package.
 
         Args:
             prompt (bool, optional): If True, prompt before updating. Defaults to True.
         """
-        if self.needs_update and (not prompt or zmtools.y_to_continue(f"A newer version ({self.latest_version}) is available. Would you like to update?")):
+        if self.needs_update and (
+            not prompt
+            or zmtools.y_to_continue(
+                f"A newer version ({self.latest_version}) is available. Would you like to update?"
+            )
+        ):
             with TemporaryDirectory() as temp_dir:
-                with zmtools.working_directory(temp_dir):
+                with zmtools.working_directory(Path(temp_dir)):
                     update_file = self._download()
                     self._update(update_file)
             print("Exiting as an update has completed")
             sys.exit()
 
     @property
     def currently_installed_version_is_unreleased(self) -> bool:
         # Override me!
         # This property should return True if the currently installed version of a package is in development, i.e. an unreleased commit
         return False
 
     @property
     def needs_update(self) -> bool:
-        if self.current_version == "0.0.0":
-            return False
-        elif self.currently_installed_version_is_unreleased:
+        if (
+            self.current_version == "0.0.0"
+            or self.currently_installed_version_is_unreleased
+        ):
             return False
         else:
-            current_version = packaging.version.parse(self.current_version)
-            latest_version = packaging.version.parse(self.latest_version)
-            return latest_version > current_version
+            return packaging.version.parse(
+                self.latest_version
+            ) > packaging.version.parse(self.current_version)
```

### Comparing `zm-au-1.2.0/zm_au/pip_au.py` & `zm_au-2.0.0/zm_au/pip/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,53 +2,62 @@
 import os
 import subprocess
 import sys
 from typing import Optional, Union
 
 import packaging.version
 import requests
-from zetuptools import PipPackage
+from python_install_directives import PipPackage
 
-from .base_au import BaseAU
+from ..base import BaseAU
 
 
 class PipAU(BaseAU):
-
     def __init__(self, name: str, silent: bool = False) -> None:
-        # If silent, redirect output of pip to the null device
         self._pip_package = PipPackage(name)
         self.silent = silent
         super().__init__()
 
     @property
     def _o(self) -> Optional[int]:
-        # Determines what to redirect output to
+        # If silent, redirect output of pip to the null device
         if self.silent:
             return subprocess.DEVNULL
         else:
             return None
 
     def _get_current_version(self) -> str:
         return self._pip_package.version
 
     def _get_latest_version(self) -> str:
         # Hits the PyPI API to find the latest version
-        return requests.get(f"https://pypi.org/pypi/{self._pip_package.name}/json").json()["info"]["version"]
+        return requests.get(
+            f"https://pypi.org/pypi/{self._pip_package.name}/json"
+        ).json()["info"]["version"]
 
     def _update(self, update_file: Union[os.PathLike, str]) -> None:
         # Runs a `pip install` of the version found by _get_latest_version (doesn't blindly install the latest version to avoid weird race conditions)
         # Note that _download was never overridden. It does not need to be as that functionality is built into `pip install`
-        subprocess.run([sys.executable, "-m", "pip", "install",
-                        f"{self._pip_package.name}=={self.latest_version}"], stdout=self._o)
+        subprocess.run(
+            [
+                sys.executable,
+                "-m",
+                "pip",
+                "install",
+                f"{self._pip_package.name}=={self.latest_version}",
+            ],
+            stdout=self._o,
+        )
         try:
             importlib.import_module(
-                f"{self._pip_package.name}.install_directives")
-            has_id = True
+                f"{self._pip_package.name}.python_install_directives"
+            )
         except ModuleNotFoundError:
             has_id = False
+        else:
+            has_id = True
         if has_id:
-            subprocess.run(
-                ["install-directives", self._pip_package.name, "install"])
+            subprocess.run(["install-directives", self._pip_package.name, "install"])
 
     @property
     def currently_installed_version_is_unreleased(self) -> bool:
-        return bool(packaging.version.parse(self.current_version).local) or self._pip_package.editable
+        return bool(packaging.version.parse(self.current_version).local)
```

### Comparing `zm-au-1.2.0/zm_au/pip_github_au.py` & `zm_au-2.0.0/zm_au/pip/github.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,76 +2,98 @@
 import json
 import os
 import subprocess
 import sys
 from typing import Optional
 
 import packaging.version
-from zetuptools import PipPackage
+from python_install_directives import PipPackage
 
-from .base_au import BaseAU, UpdateException
+from ..base import BaseAU, UpdateException
 
 
 class PipGitHubAU(BaseAU):
-
-    def __init__(self, name: str, github_location: str, check_prerelease: bool = False, dist: str = "whl", silent: bool = False):
-        # If silent, redirect output of pip to the null device
-        # Other parameters tell which uploads to look for and where (note that github_location's format is like "zmarffy/au")
+    def __init__(
+        self,
+        name: str,
+        github_location: str,
+        check_prerelease: bool = False,
+        dist: str = "whl",
+        silent: bool = False,
+    ):
+        # These parameters tell which uploads to look for and where (note that github_location's format is like "zmarffy/au")
         self._pip_package = PipPackage(name)
         self.github_location = github_location
         self.check_prerelease = check_prerelease
         self.dist = dist
         self.silent = silent
         super().__init__()
 
     @property
     def _o(self) -> Optional[int]:
-        # Determines what to redirect output to
+        # If silent, redirect output of pip to the null device
         if self.silent:
             return subprocess.DEVNULL
         else:
             return None
 
     def _get_current_version(self) -> str:
         return self._pip_package.version
 
     def _get_latest_version(self) -> str:
         # Uses `gh api` to find the latest version
         try:
-            d = json.loads(subprocess.check_output(
-                ["gh", "api", f"repos/{self.github_location}/releases"]))
+            d = json.loads(
+                subprocess.check_output(
+                    ["gh", "api", f"repos/{self.github_location}/releases"]
+                )
+            )
         except subprocess.CalledProcessError:
             raise UpdateException(
-                f"Either {self.github_location} doesn't exist or you need to authorize with GitHub (run `gh auth login`) before attempting to check for updates for it")
+                f"Either {self.github_location} doesn't exist or you need to authorize with GitHub (run `gh auth login`) before attempting to check for updates for it"
+            )
         if not self.check_prerelease:
             latest = next(x for x in d if not x["prerelease"])
         else:
             latest = d[0]
         return latest["tag_name"]
 
     def _download(self) -> str:
         # Uses `gh release download` to download the version found from _get_latest_version (doesn't blindly install the latest version to avoid a super rare race condition)
-        subprocess.run(["gh", "release", "download", self.latest_version,
-                        "-R", self.github_location, "-p", f"*.{self.dist}"], stdout=self._o)
+        subprocess.run(
+            [
+                "gh",
+                "release",
+                "download",
+                self.latest_version,
+                "-R",
+                self.github_location,
+                "-p",
+                f"*.{self.dist}",
+            ],
+            stdout=self._o,
+        )
         files = os.listdir()
         if len(files) != 1:
             raise ValueError(
-                f"Ambiguous install instructions as multiple files were downloaded. Files: {files}")
+                f"Ambiguous install instructions as multiple files were downloaded. Files: {files}"
+            )
         return files[0]
 
     def _update(self, update_file: str):
         # Installs a file with `pip install`
-        subprocess.run([sys.executable, "-m", "pip",
-                        "install", update_file], stdout=self._o)
+        subprocess.run(
+            [sys.executable, "-m", "pip", "install", update_file], stdout=self._o
+        )
         try:
             importlib.import_module(
-                f"{self._pip_package.name}.install_directives")
+                f"{self._pip_package.name}.python_install_directives"
+            )
             has_id = True
         except ModuleNotFoundError:
             has_id = False
         if has_id:
-            subprocess.run(
-                ["install-directives", self._pip_package.name, "install"])
+            subprocess.run(["install-directives", self._pip_package.name, "install"])
 
     @property
     def currently_installed_version_is_unreleased(self) -> bool:
-        return bool(packaging.version.parse(self.current_version).local) or self._pip_package.editable
+        return bool(packaging.version.parse(self.current_version).local)
```

### Comparing `zm-au-1.2.0/setup.py` & `zm_au-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,64 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: zm-au
+Version: 2.0.0
+Summary: Auto-updater for programs
+Home-page: https://github.com/zmarffy/au
+License: MIT
+Author: Zeke Marffy
+Author-email: zmarffy@yahoo.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: install-directives (>=1.0.0,<2.0.0)
+Requires-Dist: packaging (>=22.0,<23.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: zmtools (>=3.0.0,<4.0.0)
+Project-URL: Repository, https://github.com/zmarffy/au
+Description-Content-Type: text/markdown
 
-packages = \
-['zm_au']
+# `zm-au`
 
-package_data = \
-{'': ['*']}
+`zm-au` is a developer tool that provides an auto-updating API for programs. Note that this can be a bad idea for many reasons, so you should probably ask the user first.
 
-install_requires = \
-['packaging>=20.9,<21.0', 'zetuptools>=4.0.1,<5.0.0', 'zmtools>=2.0.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'zm-au',
-    'version': '1.2.0',
-    'description': 'Auto-updater for programs',
-    'long_description': '# `zm-au`\n\n`zm-au` is a developer tool that provides an auto-updating API for programs. Note that this can be a bad idea for many reasons, so you should probably ask the user first.\n\nSorry for prefixing the name with "zm", but I\'m sure I\'ll have to do that again as I have no creative names for anything anymore.\n\n## Usage\n\n`zm-au` comes with two useful auto-updaters, `PipAU` and `PipGitHubAU`, and a class to base an auto-updater off of.\n\nLet\'s say you are creating a Python package called `skippitybop` and you want it to notify the user when there is an update available on PyPI for it. Simply insert this code where you want the update check to happen.\n\n```python\nfrom zm_au import PipAU\n\nupdater = PipAU("skippitybop")\nupdater.update(prompt=True)\n```\n\nWhen the code is run, if there is an update available on PyPI, the user will be prompted to install it via `pip`. If the user chooses to install it, the program will exit on success. Or failure, for that matter.\n\nTake a guess what `prompt=False` would do.\n\nLet\'s say you are creating a Python package called `boppityskip` on bigboi\'s GitHub repo and you want it to notify the user when there is an update available on GitHub releases for it, probably because the package is private and not on PyPI. Insert this code where you want the update check to happen.\n\n```python\nfrom zm_au import PipGitHubAU\n\nupdater = PipGitHubAU("boppityskip", "bigboi/boppityskip", check_prerelease=True, dist="whl")\nupdater.update(prompt=True)\n```\n\nWhen the code is run, if there is an update available on GitHub releases (including prereleases) that is a `whl` file, the user will be prompted to install it via `pip`. Again, if the user chooses to install it, the program will exit on success or failure.\n\nYou can build your own AUs by making a class that inherits from `BaseAU`. Override the following functions as such.\n\n- `_get_current_version` - Must return the current version of the package\n- `_get_latest_version` - Must return the latest version of the package\n- `_download` - Must download the package and return the filename of the downloaded file\n- `_update` - Must install a package whose location is passed via the only parameter of this function\n\nBe smart about how you use this!\n',
-    'author': 'Zeke Marffy',
-    'author_email': 'zmarffy@yahoo.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/zmarffy/au',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Sorry for prefixing the name with "zm", but I'm sure I'll have to do that again as I have no creative names for anything anymore.
 
+## Usage
+
+`zm-au` comes with two useful auto-updaters, `PipAU` and `PipGitHubAU`, and a class to base an auto-updater off of.
+
+Let's say you are creating a Python package called `skippitybop` and you want it to notify the user when there is an update available on PyPI for it. Simply insert this code where you want the update check to happen.
+
+```python
+from zm_au import PipAU
+
+updater = PipAU("skippitybop")
+updater.update(prompt=True)
+```
+
+When the code is run, if there is an update available on PyPI, the user will be prompted to install it via `pip`. If the user chooses to install it, the program will exit on success. Or failure, for that matter.
+
+Take a guess what `prompt=False` would do.
+
+Let's say you are creating a Python package called `boppityskip` on bigboi's GitHub repo and you want it to notify the user when there is an update available on GitHub releases for it, probably because the package is private and not on PyPI. Insert this code where you want the update check to happen.
+
+```python
+from zm_au import PipGitHubAU
+
+updater = PipGitHubAU("boppityskip", "bigboi/boppityskip", check_prerelease=True, dist="whl")
+updater.update(prompt=True)
+```
+
+When the code is run, if there is an update available on GitHub releases (including prereleases) that is a `whl` file, the user will be prompted to install it via `pip`. Again, if the user chooses to install it, the program will exit on success or failure.
+
+You can build your own AUs by making a class that inherits from `BaseAU`. Override the following functions as such.
+
+- `_get_current_version` - Must return the current version of the package
+- `_get_latest_version` - Must return the latest version of the package
+- `_download` - Must download the package and return the filename of the downloaded file
+- `_update` - Must install a package whose location is passed via the only parameter of this function
+
+Be smart about how you use this!
 
-setup(**setup_kwargs)
```

