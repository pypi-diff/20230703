# Comparing `tmp/termkit-0.2.0a2.tar.gz` & `tmp/termkit-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termkit-0.2.0a2.tar", max compression
+gzip compressed data, was "termkit-0.2.0a3.tar", max compression
```

## Comparing `termkit-0.2.0a2.tar` & `termkit-0.2.0a3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a2/LICENSE
--rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a2/README.md
--rw-r--r--   0        0        0      620 2023-06-25 21:18:51.732952 termkit-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0      237 2023-06-21 20:43:42.356239 termkit-0.2.0a2/termkit/__init__.py
--rw-r--r--   0        0        0     6069 2023-06-21 20:43:42.512238 termkit-0.2.0a2/termkit/arguments.py
--rw-r--r--   0        0        0    10614 2023-06-25 09:23:37.771593 termkit-0.2.0a2/termkit/components.py
--rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/exceptions.py
--rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/formatters.py
--rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/groups.py
--rw-r--r--   0        0        0     1291 2023-06-21 20:43:42.316239 termkit-0.2.0a2/termkit/helpers.py
--rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a2/termkit/tests.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 termkit-0.2.0a2/setup.py
--rw-r--r--   0        0        0     3684 1970-01-01 00:00:00.000000 termkit-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-06-12 22:04:59.365121 termkit-0.2.0a3/LICENSE
+-rw-r--r--   0        0        0     3170 2023-06-13 05:50:26.603066 termkit-0.2.0a3/README.md
+-rw-r--r--   0        0        0      697 2023-07-03 21:35:16.482914 termkit-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-21 20:43:42.356239 termkit-0.2.0a3/termkit/__init__.py
+-rw-r--r--   0        0        0     6550 2023-06-27 15:28:33.270769 termkit-0.2.0a3/termkit/arguments.py
+-rw-r--r--   0        0        0    13823 2023-07-03 06:27:45.931899 termkit-0.2.0a3/termkit/components.py
+-rw-r--r--   0        0        0      698 2023-06-12 22:04:59.369121 termkit-0.2.0a3/termkit/exceptions.py
+-rw-r--r--   0        0        0     2575 2023-06-12 22:04:59.369121 termkit-0.2.0a3/termkit/formatters.py
+-rw-r--r--   0        0        0      543 2023-06-12 22:04:59.369121 termkit-0.2.0a3/termkit/groups.py
+-rw-r--r--   0        0        0     1291 2023-06-21 20:43:42.316239 termkit-0.2.0a3/termkit/helpers.py
+-rw-r--r--   0        0        0     2052 2023-06-12 22:04:59.369121 termkit-0.2.0a3/termkit/tests.py
+-rw-r--r--   0        0        0     3879 1970-01-01 00:00:00.000000 termkit-0.2.0a3/setup.py
+-rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 termkit-0.2.0a3/PKG-INFO
```

### Comparing `termkit-0.2.0a2/LICENSE` & `termkit-0.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/README.md` & `termkit-0.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/pyproject.toml` & `termkit-0.2.0a3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 [tool.poetry]
 name = "termkit"
-version = "0.2.0a2"
+version = "0.2.0a3"
 description = "Command Line Tools with ease"
 authors = ["Thomas Mahé <contact@tmahe.dev>"]
 readme = "README.md"
 
+#[tool.poetry.scripts]
+#termkit = 'termkit.app:entry_point'
+
 [tool.poetry.dependencies]
 python = "^3.7"
+pyyaml = "^6.0"
 
 [tool.poetry.group.devel.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.15"
 tox = "^4.6.0"
 
 [tool.pytest.ini_options]
```

### Comparing `termkit-0.2.0a2/termkit/arguments.py` & `termkit-0.2.0a3/termkit/arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 import typing
 from abc import ABC, abstractmethod
 from typing import Optional, Type, Any, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:  # pragma: nocover
-    from termkit.components import TermkitParser
+    from termkit.components import TermkitParser, ProfileResolver
 
 from termkit.groups import ArgumentGroup, MutuallyExclusiveGroup
 from termkit.helpers import Nargs
 
 
 class Argument(ABC):
     type: Optional[Type]
@@ -57,14 +57,21 @@
 
         if self.type is None and type_hint is None:
             self.type = str
 
         if self.help is None:
             self.help = ""
 
+        profile: ProfileResolver = parser._app._profile
+        if profile:
+            value = profile.resolve(argument_name)
+            if value is not None:
+                self.default = value
+                self.nargs = "?"
+
         self.help = f"{self.help} (%(type)s) ".strip()
 
         if self.default is not None:
             self.help = f"{self.help} (default: %(default)s) ".strip()
 
         args = self.__dict__.copy()
         del args['group']
@@ -111,14 +118,21 @@
                 self.type = type(self.default)
             else:
                 self.type = str
 
         if self.metavar is None and self.choices is None:
             self.metavar = self.type.__name__.upper()
 
+        profile: ProfileResolver = parser._app._profile
+        if profile:
+            value = profile.resolve(argument_name)
+            if value is not None:
+                self.default = value
+                self.nargs = "?"
+
         if self.help is None:
             self.help = ""
 
         if self.default is not None:
             self.required = False
             self.help = f"{self.help} (default: %(default)s)".strip()
```

### Comparing `termkit-0.2.0a2/termkit/components.py` & `termkit-0.2.0a3/termkit/components.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # SPDX-FileCopyrightText: 2023 Thomas Mahé <contact@tmahe.dev>
 
 import argparse
 import inspect
+import logging
 import os
 import sys
 import typing
 from abc import ABC
+from pathlib import Path
 from typing import Optional, Callable, Union, Dict, Any
 
+import yaml
+
 from termkit.helpers import get_callback_arguments
 from termkit.groups import ArgumentGroup, MutuallyExclusiveGroup
 
 from termkit.formatters import TermkitDefaultFormatter
 from termkit.arguments import Argument
 from termkit.exceptions import TermkitError, InconsistentTypingError
 
@@ -26,15 +30,16 @@
 class Termkit(Component):
     _callback: Optional[Callable]
     _childs: typing.List[Component]
 
     def __init__(self,
                  name: Optional[str] = None,
                  callback: Optional[Callable] = None,
-                 description: Optional[str] = None):
+                 description: Optional[str] = None,
+                 named_profile: bool = False):
 
         # Legacy argparse default for prog name
         if name is None:
             name = os.path.basename(sys.argv[0])
 
         if callback is not None and not inspect.isfunction(callback):
             raise TermkitError("termkit.Command callback must be a function")
@@ -42,24 +47,32 @@
         self.description = description
 
         if description is None:
             self.help = None
         else:
             self.help = description.splitlines()[0]
 
+        self._profile = None
+        if named_profile:
+            self._profile = ProfileResolver()
+
         self.name = name
 
         self._callback = callback
         self._childs = list()
 
     def add(self, app_or_command: typing.Union[Component, Callable]):
         # Adding sub-app
         if isinstance(app_or_command, Termkit):
             if app_or_command.name == os.path.basename(sys.argv[0]):
                 raise TermkitError('cannot add unnamed Termkit application')
+            if self._profile:
+                app_or_command._profile = ProfileResolver(ctx=self._profile.ctx + [app_or_command.name],
+                                                          content=self._profile._content,
+                                                          selected=self._profile._selected)
             self._childs.append(app_or_command)
 
         # Adding command
         elif isinstance(app_or_command, Command):
             self._childs.append(app_or_command)
 
         # Adding function
@@ -77,16 +90,20 @@
             self._childs.pop()
             raise TermkitError(f"duplicated command or sub-app name {duplicates} in application '{self.name}'")
 
     def command(self, name: Optional[str] = None):
         def _decorated_callable(callback: Callable, _name=name):
             if _name is None:
                 _name = callback.__name__
-            self._childs.append(Command(name=_name,
-                                        callback=callback))
+            c = Command(name=_name, callback=callback)
+            if self._profile:
+                c._profile = ProfileResolver(ctx=self._profile.ctx + [_name],
+                                             content=self._profile._content,
+                                             selected=self._profile._selected)
+            self._childs.append(c)
             return callback
 
         return _decorated_callable
 
     def callback(self):
         def _decorated_callable(callback: Callable):
             if inspect.isfunction(callback):
@@ -119,24 +136,81 @@
                  name: str,
                  callback: Callable):
         if not inspect.isfunction(callback):
             raise TermkitError("termkit.Command callback must be a function")
 
         self.name = str(name)
         self._callback = callback
+        self._profile = None
 
         doc = inspect.getdoc(callback)
         if doc is None:
             self.help = ""
             self.description = ""
         else:
             self.help = doc.splitlines()[0]
             self.description = doc
 
 
+class ProfileResolver:
+
+    @staticmethod
+    def get_selected_profile():
+        parser = argparse.ArgumentParser(add_help=False)
+        parser.add_argument("--profile", default="default", nargs="*")
+        args, unk = parser.parse_known_args()
+        return args.profile
+
+    def __init__(self, ctx=None, content=None, selected=None):
+        self.ctx = ctx
+        if self.ctx is None:
+            self.ctx = []
+
+        self.app_name = os.path.basename(sys.argv[0])
+        self._files = [
+            Path.home().joinpath('.config').joinpath(self.app_name).joinpath("profile.yaml"),
+            Path.home().joinpath('.config').joinpath(self.app_name).joinpath("profile.yml"),
+            Path.cwd().joinpath(f'.{self.app_name}.yaml'),
+            Path.cwd().joinpath(f'.{self.app_name}.yml'),
+        ]
+        if content is not None:
+            self._content = content
+        else:
+            logger = logging.getLogger("termkit.components.ProfileResolver")
+            self._content = []
+            for file in self._files:
+                if os.path.exists(file):
+                    try:
+                        with open(file, 'r') as f:
+                            self._content.append(yaml.safe_load(f.read()))
+                    except yaml.YAMLError:
+                        logger.warning(f"[WARNING] Unable to parse {file}, profiles would not be imported.")
+                        continue
+
+        self._profiles = []
+        for e in self._content:
+            self._profiles += e.keys()
+
+        self._selected = selected
+        if self._selected is None:
+            self._selected = self.get_selected_profile()
+
+    def resolve(self, argument_name):
+        out = None
+        for p in self._selected:
+            for f in self._content:
+                ctx = f.get(p, {})
+                for e in self.ctx:
+                    ctx = ctx.get(e, {})
+                    for name, value in ctx.items():
+                        if name == argument_name:
+                            out = value
+        return out
+
+
 class TermkitParser(argparse.ArgumentParser):
     _argument_groups: Dict[Union[ArgumentGroup, MutuallyExclusiveGroup], Any]
 
     def __init__(self, app: Termkit, *args, **kwargs):
         if not isinstance(app, Component):
             raise TermkitError(f"TermkitParser.app expected object of type [Termkit | Command], {type(app)} provided")
 
@@ -190,14 +264,18 @@
 
             for child in app._childs:
                 p.add_parser(app=child, name=child.name, help=child.help, description=child.description, depth=self._depth+1)
 
     def _populate_command(self, command: Command):
         self.add_argument(f'__TERMKIT_CALLBACK_{self._depth}', action="store_const", const=command._callback,
                           help=argparse.SUPPRESS)
+        if command._profile:
+            self.add_argument(f'--profile', metavar="NAME", nargs="+", default="default",
+                              help=f"Named profile to use\n(selected: {command._profile._selected})",
+                              choices=command._profile._profiles)
         if sys.version_info >= (3, 9):
             type_hints = typing.get_type_hints(command._callback, include_extras=True)
         else:
             type_hints = typing.get_type_hints(command._callback)  # pragma: nocover
 
         for arg_name, arg_spec in inspect.signature(command._callback).parameters.items():
 
@@ -250,15 +328,16 @@
         if isinstance(group, MutuallyExclusiveGroup) and group.parent is not None:
             parent_group = self.add_argument_group(group=group.parent)
 
         if isinstance(group, MutuallyExclusiveGroup):
             self._argument_groups[group] = parent_group.add_mutually_exclusive_group(required=group.required)
 
         if isinstance(group, ArgumentGroup):
-            self._argument_groups[group] = super(self.__class__, self).add_argument_group(title=group.title, description=group.description)
+            self._argument_groups[group] = super(self.__class__, self).add_argument_group(title=group.title,
+                                                                                          description=group.description)
 
         return self._argument_groups[group]
 
 
 def run(func_or_app: Union[Callable, Termkit],
         argcomplete: bool = False):
     if inspect.isfunction(func_or_app):
```

### Comparing `termkit-0.2.0a2/termkit/exceptions.py` & `termkit-0.2.0a3/termkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/termkit/formatters.py` & `termkit-0.2.0a3/termkit/formatters.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/termkit/groups.py` & `termkit-0.2.0a3/termkit/groups.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/termkit/helpers.py` & `termkit-0.2.0a3/termkit/helpers.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/termkit/tests.py` & `termkit-0.2.0a3/termkit/tests.py`

 * *Files identical despite different names*

### Comparing `termkit-0.2.0a2/setup.py` & `termkit-0.2.0a3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 packages = \
 ['termkit']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['pyyaml>=6.0,<7.0']
+
 setup_kwargs = {
     'name': 'termkit',
-    'version': '0.2.0a2',
+    'version': '0.2.0a3',
     'description': 'Command Line Tools with ease',
     'long_description': '<p align="center">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner.png#gh-dark-mode-only" width="450">\n    <img alt="Termkit" title="Termkit" src="docs/images/banner_light.png#gh-light-mode-only" width="450">\n</p>\n<div align="center">\n  <b><i>Command Line Tools with... ease.</i></b>\n<hr>\n\n[![Tests](https://github.com/thmahe/termkit/actions/workflows/tests.yml/badge.svg)](https://github.com/thmahe/termkit/actions/workflows/tests.yml)\n[![codecov](https://codecov.io/github/thmahe/termkit/branch/master/graph/badge.svg?token=o7UVrOsoq4)](https://codecov.io/github/thmahe/termkit)\n![PyPI](https://img.shields.io/pypi/v/termkit)\n![Platforms](https://img.shields.io/badge/platforms-Linux%20%7C%20MacOS%20%7C%20Windows-lightgrey)\n\n</div>\n\n## Table of Contents\n\n- [Introduction](#introduction)\n- [Features](#features)\n- [Requirement](#requirement)\n- [Installation](#installation)\n- [Examples](#examples)\n- [Feedback](#feedback)\n- [Acknowledgments](#acknowledgments)\n\n## Introduction\n\nTermkit is a framework for building command line interface applications using functions \nand type hints [[PEP 484]](https://peps.python.org/pep-0484/). \n**Solely written using [Python Standard Library](https://docs.python.org/3/library/)** and will always be to ensure\nminimal dependency footprint within your project.\n\nIn few words, Termkit is designed to be the foundation of serious CLI tools.\n\n## Features\n\nA few of the things you can do with Termkit:\n\n* Build CLI from functional code\n* Create fast prototypes using implicit arguments\n* Helpers populated from docstrings\n* Named profile for pre-populated arguments\n* Autocompletion through [argcomplete](https://pypi.org/project/argcomplete/) module\n* Cross-platforms\n\n## Requirement\n* Python 3.7 or higher\n\n*Yes... that\'s about it !* \n\n### Compatibility matrix\n\n|          OS | Python 3.6 |     Python 3.7     |     Python 3.8     |     Python 3.9     |    Python 3.10     |    Python 3.11     |    Python 3.12    |\n|------------:|:----------:|:------------------:|:------------------:|:------------------:|:------------------:|:------------------:|:-----------------:|\n|   **Linux** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n|   **MacOS** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n| **Windows** |    :x:     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_plus_sign: |\n\n\n## Installation\n\nTermkit is published as a [Python package](https://pypi.org/project/termkit) and can be installed with pip.\n\nOpen up a terminal and install Termkit with:\n```shell\npip install termkit\n```\n\n## Examples\n\n### Greeting application\n\n```python\n# greet.py\nimport termkit\n\ndef greet(name):\n    print(f\'Hello {name} !\')\n\nif __name__ == \'__main__\':\n    termkit.run(greet)\n```\n\n```\n$ python3 ./greet.py Thomas\nHello Thomas !\n```\n\n## Feedback\n\nFeel free to send me feedback by [raising an issue](https://github.com/thmahe/termkit/issues/new).\nFeature requests are always welcome.\n\n',
     'author': 'Thomas Mahé',
     'author_email': 'contact@tmahe.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `termkit-0.2.0a2/PKG-INFO` & `termkit-0.2.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: termkit
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Command Line Tools with ease
 Author: Thomas Mahé
 Author-email: contact@tmahe.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img alt="Termkit" title="Termkit" src="docs/images/banner.png#gh-dark-mode-only" width="450">
     <img alt="Termkit" title="Termkit" src="docs/images/banner_light.png#gh-light-mode-only" width="450">
 </p>
 <div align="center">
```

