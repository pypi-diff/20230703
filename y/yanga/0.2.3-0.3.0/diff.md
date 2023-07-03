# Comparing `tmp/yanga-0.2.3.tar.gz` & `tmp/yanga-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanga-0.2.3.tar", max compression
+gzip compressed data, was "yanga-0.3.0.tar", max compression
```

## Comparing `yanga-0.2.3.tar` & `yanga-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-07-03 16:56:32.184599 yanga-0.2.3/LICENSE
--rw-r--r--   0        0        0     4695 2023-07-03 16:56:32.184599 yanga-0.2.3/README.md
--rw-r--r--   0        0        0     2384 2023-07-03 16:56:33.040606 yanga-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-03 16:56:33.008606 yanga-0.2.3/src/yanga/__init__.py
--rw-r--r--   0        0        0      347 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/_yrun.py
--rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/__init__.py
--rw-r--r--   0        0        0     1802 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/build.py
--rw-r--r--   0        0        0     2493 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/init.py
--rw-r--r--   0        0        0      412 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/cookiecutter.json
--rw-r--r--   0        0        0        7 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
--rw-r--r--   0        0        0     5389 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1
--rw-r--r--   0        0        0     3853 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
--rw-r--r--   0        0        0      785 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
--rw-r--r--   0        0        0      157 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
--rw-r--r--   0        0        0       34 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
--rw-r--r--   0        0        0      247 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
--rw-r--r--   0        0        0      110 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
--rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/__init__.py
--rw-r--r--   0        0        0     4221 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/docs_utils.py
--rw-r--r--   0        0        0      278 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/exceptions.py
--rw-r--r--   0        0        0     1583 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/logger.py
--rw-r--r--   0        0        0     2910 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/scoop_wrapper.py
--rw-r--r--   0        0        0     1349 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/core/subprocess.py
--rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/py.typed
--rw-r--r--   0        0        0        0 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/__init__.py
--rw-r--r--   0        0        0      851 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/build_main.py
--rw-r--r--   0        0        0      965 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/config.py
--rw-r--r--   0        0        0      477 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/environment.py
--rw-r--r--   0        0        0     3141 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/pipeline.py
--rw-r--r--   0        0        0      864 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/project.py
--rw-r--r--   0        0        0      670 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/stages.py
--rw-r--r--   0        0        0      886 2023-07-03 16:56:32.184599 yanga-0.2.3/src/yanga/ybuild/variant.py
--rw-r--r--   0        0        0      790 2023-07-03 16:56:32.188599 yanga-0.2.3/src/yanga/ymain.py
--rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-03 20:04:56.271476 yanga-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4695 2023-07-03 20:04:56.271476 yanga-0.3.0/README.md
+-rw-r--r--   0        0        0     2384 2023-07-03 20:04:57.119473 yanga-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-03 20:04:57.087473 yanga-0.3.0/src/yanga/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/_yrun.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/__init__.py
+-rw-r--r--   0        0        0     1803 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/build.py
+-rw-r--r--   0        0        0     2494 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/init.py
+-rw-r--r--   0        0        0      412 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/cookiecutter.json
+-rw-r--r--   0        0        0        7 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/.gitignore
+-rw-r--r--   0        0        0     5389 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1
+-rw-r--r--   0        0        0     3853 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py
+-rw-r--r--   0        0        0      785 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1
+-rw-r--r--   0        0        0      157 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/install.yaml
+-rw-r--r--   0        0        0       34 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/poetry.toml
+-rw-r--r--   0        0        0      247 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/yanga.yaml
+-rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/exceptions.py
+-rw-r--r--   0        0        0     1583 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/logging.py
+-rw-r--r--   0        0        0     6113 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     1350 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/core/subprocess.py
+-rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/py.typed
+-rw-r--r--   0        0        0        0 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/build_main.py
+-rw-r--r--   0        0        0      965 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/config.py
+-rw-r--r--   0        0        0      477 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/environment.py
+-rw-r--r--   0        0        0     3141 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/pipeline.py
+-rw-r--r--   0        0        0      864 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/project.py
+-rw-r--r--   0        0        0     1403 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/stages.py
+-rw-r--r--   0        0        0      886 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ybuild/variant.py
+-rw-r--r--   0        0        0      791 2023-07-03 20:04:56.275476 yanga-0.3.0/src/yanga/ymain.py
+-rw-r--r--   0        0        0     5803 1970-01-01 00:00:00.000000 yanga-0.3.0/PKG-INFO
```

### Comparing `yanga-0.2.3/LICENSE` & `yanga-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/README.md` & `yanga-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/pyproject.toml` & `yanga-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yanga"
-version = "0.2.3"
+version = "0.3.0"
 description = "Yet another ninja generator to build C/CPP projects."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/yanga"
 documentation = "https://yanga.readthedocs.io"
 classifiers = [
```

### Comparing `yanga-0.2.3/src/yanga/commands/build.py` & `yanga-0.3.0/src/yanga/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import ArgumentParser, Namespace
 from dataclasses import dataclass, field
 from pathlib import Path
 
 from mashumaro import DataClassDictMixin
 
 from yanga.core.cmd_line import Command, register_arguments_for_config_dataclass
-from yanga.core.logger import logger, time_it
+from yanga.core.logging import logger, time_it
 from yanga.ybuild.build_main import YangaBuild
 from yanga.ybuild.environment import BuildEnvironment
 
 
 @dataclass
 class BuildCommandConfig(DataClassDictMixin):
     variant_name: str = field(metadata={"help": "SPL variant name."})
```

### Comparing `yanga-0.2.3/src/yanga/commands/init.py` & `yanga-0.3.0/src/yanga/commands/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tempfile import TemporaryDirectory
 
 from cookiecutter.main import cookiecutter
 from mashumaro import DataClassDictMixin
 
 from yanga.core.cmd_line import Command
 from yanga.core.exceptions import UserNotificationException
-from yanga.core.logger import logger, time_it
+from yanga.core.logging import logger, time_it
 
 
 @dataclass
 class InitCommandConfig(DataClassDictMixin):
     project_dir: Path
 
     @classmethod
```

### Comparing `yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1` & `yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py` & `yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/build.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1` & `yanga-0.3.0/src/yanga/commands/project-template/{{ cookiecutter.project_dir_name }}/cleanup.ps1`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/core/cmd_line.py` & `yanga-0.3.0/src/yanga/core/cmd_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import dataclasses
 from abc import ABC, abstractmethod
 from argparse import ArgumentError, ArgumentParser, Namespace
 from typing import Dict, List, Type
 
 from .docs_utils import fulfills
-from .logger import logger
+from .logging import logger
 
 
 class Command(ABC):
     def __init__(self, name: str, description: str) -> None:
         self.name = name
         self.description = description
         self.parser: ArgumentParser
```

### Comparing `yanga-0.2.3/src/yanga/core/docs_utils.py` & `yanga-0.3.0/src/yanga/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/core/logger.py` & `yanga-0.3.0/src/yanga/core/logging.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/core/subprocess.py` & `yanga-0.3.0/src/yanga/core/subprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import subprocess  # nosec
 from pathlib import Path
 from typing import List, Optional
 
 from .exceptions import UserNotificationException
-from .logger import logger
+from .logging import logger
 
 
 def get_app_path(app_name: str) -> Optional[Path]:
     """Return the path to the app if it is in the PATH, otherwise return None."""
     app_path = shutil.which(app_name)
     return Path(app_path) if app_path else None
```

### Comparing `yanga-0.2.3/src/yanga/ybuild/build_main.py` & `yanga-0.3.0/src/yanga/ybuild/build_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yanga.core.logger import logger
+from yanga.core.logging import logger
 from yanga.ybuild.config import YangaConfig
 from yanga.ybuild.environment import BuildEnvironment
 from yanga.ybuild.pipeline import PipelineLoader, StageRunner
 
 
 class YangaBuild:
     def __init__(self, environment: BuildEnvironment) -> None:
```

### Comparing `yanga-0.2.3/src/yanga/ybuild/config.py` & `yanga-0.3.0/src/yanga/ybuild/config.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/ybuild/pipeline.py` & `yanga-0.3.0/src/yanga/ybuild/pipeline.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/ybuild/project.py` & `yanga-0.3.0/src/yanga/ybuild/project.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/ybuild/stages.py` & `yanga-0.3.0/src/yanga/ybuild/stages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 from typing import List
 
-from yanga.core.logger import logger
+from yanga.core.logging import logger
+from yanga.core.scoop_wrapper import ScoopWrapper
 from yanga.ybuild.environment import BuildEnvironment
 from yanga.ybuild.pipeline import Stage
 
 
 class YangaInstall(Stage):
     def __init__(self, environment: BuildEnvironment, group_name: str) -> None:
         super().__init__(environment, group_name)
@@ -17,7 +18,29 @@
         )
 
     def get_dependencies(self) -> List[Path]:
         return []
 
     def get_outputs(self) -> List[Path]:
         return []
+
+
+class YangaScoopInstall(Stage):
+    def __init__(self, environment: BuildEnvironment, group_name: str) -> None:
+        super().__init__(environment, group_name)
+        self.logger = logger.bind()
+
+    @property
+    def scoop_file(self) -> Path:
+        return self.environment.project_root_dir.joinpath("scoopfile.json")
+
+    def run(self) -> None:
+        self.logger.info(
+            f"Run {self.__class__.__name__} stage. Output dir: {self.output_dir}"
+        )
+        ScoopWrapper().install(self.scoop_file)
+
+    def get_dependencies(self) -> List[Path]:
+        return [self.scoop_file]
+
+    def get_outputs(self) -> List[Path]:
+        return []
```

### Comparing `yanga-0.2.3/src/yanga/ybuild/variant.py` & `yanga-0.3.0/src/yanga/ybuild/variant.py`

 * *Files identical despite different names*

### Comparing `yanga-0.2.3/src/yanga/ymain.py` & `yanga-0.3.0/src/yanga/ymain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from sys import argv
 
 from yanga.commands.build import BuildCommand
 from yanga.commands.init import InitCommand
 from yanga.core.cmd_line import CommandLineHandlerBuilder
 from yanga.core.exceptions import UserNotificationException
-from yanga.core.logger import logger, setup_logger, time_it
+from yanga.core.logging import logger, setup_logger, time_it
 
 
 @time_it()
 def do_run() -> None:
     logger.debug("Starting yanga")
     builder = CommandLineHandlerBuilder()
     builder.add_command(BuildCommand()).add_command(InitCommand())
```

### Comparing `yanga-0.2.3/PKG-INFO` & `yanga-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanga
-Version: 0.2.3
+Version: 0.3.0
 Summary: Yet another ninja generator to build C/CPP projects.
 Home-page: https://github.com/cuinixam/yanga
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yanga Version: 0.2.3 Summary: Yet another ninja
+Metadata-Version: 2.1 Name: yanga Version: 0.3.0 Summary: Yet another ninja
 generator to build C/CPP projects. Home-page: https://github.com/cuinixam/yanga
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

