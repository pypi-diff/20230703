# Comparing `tmp/uasset_dump-0.0.4.tar.gz` & `tmp/uasset_dump-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uasset_dump-0.0.4.tar", max compression
+gzip compressed data, was "uasset_dump-0.0.5.tar", max compression
```

## Comparing `uasset_dump-0.0.4.tar` & `uasset_dump-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      306 2023-07-03 08:19:28.005425 uasset_dump-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 uasset_dump-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     3876 2023-07-03 07:33:54.680171 uasset_dump-0.0.4/README.md
--rw-r--r--   0        0        0     1039 2023-07-03 08:23:51.764851 uasset_dump-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/ue/cli/__init__.py
--rwxr-xr-x   0        0        0     2616 2023-07-03 08:21:18.490361 uasset_dump-0.0.4/src/bootloader/ue/cli/uassetdump.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.4/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0     4797 2023-04-05 15:31:25.693554 uasset_dump-0.0.4/src/bootloader/ue/constant/uasset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.4/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0     2914 2023-06-14 02:27:45.682247 uasset_dump-0.0.4/src/bootloader/ue/model/uasset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/ue/utils/__init__.py
--rw-r--r--   0        0        0     5496 2023-07-03 08:21:18.479007 uasset_dump-0.0.4/src/bootloader/ue/utils/uasset_dump.py
--rw-r--r--   0        0        0     5079 1970-01-01 00:00:00.000000 uasset_dump-0.0.4/setup.py
--rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 uasset_dump-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-03 10:22:41.399896 uasset_dump-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 uasset_dump-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     3959 2023-07-03 08:35:15.010465 uasset_dump-0.0.5/README.md
+-rw-r--r--   0        0        0     1038 2023-07-03 10:22:41.395717 uasset_dump-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.5/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.5/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.5/src/bootloader/ue/cli/__init__.py
+-rwxr-xr-x   0        0        0     2616 2023-07-03 08:21:18.490361 uasset_dump-0.0.5/src/bootloader/ue/cli/uassetdump.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.5/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0     4797 2023-04-05 15:31:25.693554 uasset_dump-0.0.5/src/bootloader/ue/constant/uasset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.5/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0     2914 2023-06-14 02:27:45.682247 uasset_dump-0.0.5/src/bootloader/ue/model/uasset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.5/src/bootloader/ue/utils/__init__.py
+-rw-r--r--   0        0        0     5496 2023-07-03 08:21:18.479007 uasset_dump-0.0.5/src/bootloader/ue/utils/uasset_dump.py
+-rw-r--r--   0        0        0     5172 1970-01-01 00:00:00.000000 uasset_dump-0.0.5/setup.py
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 uasset_dump-0.0.5/PKG-INFO
```

### Comparing `uasset_dump-0.0.4/LICENSE.md` & `uasset_dump-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/README.md` & `uasset_dump-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -102,9 +102,17 @@
   },
   (...)
 ]
 ```
 
 ```shell
 export UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject
-`\"(find "/Users/Shared/Epic Games/UE_5.1" -name "UnrealEditor-Cmd")\"` "$UNREAL_ENGINE_PROJECT_PATH" -ExecutePythonScript="run.py"
+
+"`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \
+    "$UNREAL_ENGINE_PROJECT_PATH" \
+    -run=pythonscript \
+    -stdout \
+    -Unattended \
+    -script="/Users/admin/Downloads/run.py"
+
+echo $?;
 ```
```

### Comparing `uasset_dump-0.0.4/pyproject.toml` & `uasset_dump-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 ]
 keywords = ["cli", "tool", "utility", "unreal", "engine", "asset", "inventory", "dump", "json"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "uasset-dump"
 packages = [{ include = "bootloader", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/bootloader-studio/cli-uasset-dump"
-version = "0.0.4"
+version = "0.0.5"
 
 [tool.poetry.dependencies]
-perseus-core-library = "^1.19.2"
-python = "^3.10"
+perseus-core-library = "^1.19.3"
+python = "^3.9"
 
 [tool.poetry.scripts]
 ueprjver = 'bootloader.ue.cli.uassetdump:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uasset_dump-0.0.4/src/bootloader/__init__.py` & `uasset_dump-0.0.5/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/__init__.py` & `uasset_dump-0.0.5/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/cli/__init__.py` & `uasset_dump-0.0.5/src/bootloader/ue/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/cli/uassetdump.py` & `uasset_dump-0.0.5/src/bootloader/ue/cli/uassetdump.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/constant/__init__.py` & `uasset_dump-0.0.5/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/constant/uasset.py` & `uasset_dump-0.0.5/src/bootloader/ue/constant/uasset.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/model/__init__.py` & `uasset_dump-0.0.5/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/model/uasset.py` & `uasset_dump-0.0.5/src/bootloader/ue/model/uasset.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/utils/__init__.py` & `uasset_dump-0.0.5/src/bootloader/ue/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/src/bootloader/ue/utils/uasset_dump.py` & `uasset_dump-0.0.5/src/bootloader/ue/utils/uasset_dump.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.4/setup.py` & `uasset_dump-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,32 @@
  'bootloader.ue.model',
  'bootloader.ue.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['perseus-core-library>=1.19.2,<2.0.0']
+['perseus-core-library>=1.19.3,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ueprjver = bootloader.ue.cli.uassetdump:run']}
 
 setup_kwargs = {
     'name': 'uasset-dump',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Command-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure',
-    'long_description': '# Unreal Engine Assets Dump\n\nCommand-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure.\n\n## Development\n\n### Poetry\n\n_Unreal Engine Assets Dump_ project used Poetry to declare all its dependencies.  [Poetry](https://python-poetry.org/) is a python dependency management tool to manage dependencies, packages, and libraries in your python project.\n\nWe need to create the Python virtual environment using Poetry:\n\n```shell\npoetry env use /Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3\n```\n\nWe can enter this virtual environment and install all the required dependencies:\n\n```shell\npoetry shell\npoetry update\n```\n\n\n## Publication\n\nTo publish a new version of the _Unreal Engine Assets Dump_ library to [Pypi](https://pypi.org/), we need to execute the following command:\n\n```shell\npoetry publish --build --username $PYPI_USERNAME --password $PYPI_PASSWORD\n```\n\nWhere the environment variables:\n\n- `$PYPI_USERNAME`: The value `__token__`\n- `$PYPI_PASSWORD`: The [API token](https://pypi.org/manage/account/token/) used to authenticate when uploading packages to PyPI (e.g., `pypi-...`)\n\nWe generally defined a `.env` file and add these environment variables:\n\n```text\n# Copyright (C) 2023 Bootloader.  All rights reserved.\n#\n# This software is the confidential and proprietary information of\n# Bootloader or one of its subsidiaries.  You shall not disclose this\n# confidential information and shall use it only in accordance with the\n# terms of the license agreement or other applicable agreement you\n# entered into with Bootloader.\n#\n# BOOTLOADER MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE\n# SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT\n# NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR\n# A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE\n# LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF\n# USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.\n\n# The Python Package Index (PyPI) API token to authenticate when\n# uploading this package to PyPI.\nPYPI_USERNAME=__token__\nPYPI_PASSWORD=pypi-(...)\n```\n\n\n## Installation\n\nTo install _Unreal Engine Assets Dump_ library to Unreal Engine, execute the following command.\n\n```shell\n/Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n/Users/Shared/Epic\\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n```\n\n/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Content\n\n## Execution\n\nThen we can load our Unreal Engine project in Unreal Engine Editor and execute the following Python instructions in the Output Log drawer:\n\n```shell\nfrom bootloader.ue.utils import uasset_dump\nuasset_dump.dump_assets(\'/Users/dcaune/Devel/Bootloader/bootloader-human-trainer-ar5/Content\')\n```\n\nThis prints long JSON data.  For instance:\n\n```json\n[\n  {\n    "asset_name": "A_d2_ChangeOutfit_01",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_01",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  {\n    "asset_name": "A_d2_ChangeOutfit_02",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_02",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  (...)\n]\n```\n\n```shell\nexport UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject\n`\\"(find "/Users/Shared/Epic Games/UE_5.1" -name "UnrealEditor-Cmd")\\"` "$UNREAL_ENGINE_PROJECT_PATH" -ExecutePythonScript="run.py"\n```',
+    'long_description': '# Unreal Engine Assets Dump\n\nCommand-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure.\n\n## Development\n\n### Poetry\n\n_Unreal Engine Assets Dump_ project used Poetry to declare all its dependencies.  [Poetry](https://python-poetry.org/) is a python dependency management tool to manage dependencies, packages, and libraries in your python project.\n\nWe need to create the Python virtual environment using Poetry:\n\n```shell\npoetry env use /Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3\n```\n\nWe can enter this virtual environment and install all the required dependencies:\n\n```shell\npoetry shell\npoetry update\n```\n\n\n## Publication\n\nTo publish a new version of the _Unreal Engine Assets Dump_ library to [Pypi](https://pypi.org/), we need to execute the following command:\n\n```shell\npoetry publish --build --username $PYPI_USERNAME --password $PYPI_PASSWORD\n```\n\nWhere the environment variables:\n\n- `$PYPI_USERNAME`: The value `__token__`\n- `$PYPI_PASSWORD`: The [API token](https://pypi.org/manage/account/token/) used to authenticate when uploading packages to PyPI (e.g., `pypi-...`)\n\nWe generally defined a `.env` file and add these environment variables:\n\n```text\n# Copyright (C) 2023 Bootloader.  All rights reserved.\n#\n# This software is the confidential and proprietary information of\n# Bootloader or one of its subsidiaries.  You shall not disclose this\n# confidential information and shall use it only in accordance with the\n# terms of the license agreement or other applicable agreement you\n# entered into with Bootloader.\n#\n# BOOTLOADER MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE\n# SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT\n# NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR\n# A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE\n# LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF\n# USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.\n\n# The Python Package Index (PyPI) API token to authenticate when\n# uploading this package to PyPI.\nPYPI_USERNAME=__token__\nPYPI_PASSWORD=pypi-(...)\n```\n\n\n## Installation\n\nTo install _Unreal Engine Assets Dump_ library to Unreal Engine, execute the following command.\n\n```shell\n/Users/Shared/Epic\\ Games/UE_5.1/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n/Users/Shared/Epic\\ Games/UE_5.2/Engine/Binaries/ThirdParty/Python3/Mac/bin/python3 -m pip install --upgrade uasset-dump\n```\n\n/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Content\n\n## Execution\n\nThen we can load our Unreal Engine project in Unreal Engine Editor and execute the following Python instructions in the Output Log drawer:\n\n```shell\nfrom bootloader.ue.utils import uasset_dump\nuasset_dump.dump_assets(\'/Users/dcaune/Devel/Bootloader/bootloader-human-trainer-ar5/Content\')\n```\n\nThis prints long JSON data.  For instance:\n\n```json\n[\n  {\n    "asset_name": "A_d2_ChangeOutfit_01",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_01",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  {\n    "asset_name": "A_d2_ChangeOutfit_02",\n    "asset_class_path": "/Script/Engine/AnimSequence",\n    "package_name": "/Game/ArtAssets/Pets/QuadrupedDog/Animations/A_d2_ChangeOutfit_02",\n    "dependencies": [\n      "/Game/ArtAssets/Pets/QuadrupedDog/Mesh/S_d2"\n    ]\n  },\n  (...)\n]\n```\n\n```shell\nexport UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject\n\n"`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \\\n    "$UNREAL_ENGINE_PROJECT_PATH" \\\n    -run=pythonscript \\\n    -stdout \\\n    -Unattended \\\n    -script="/Users/admin/Downloads/run.py"\n\necho $?;\n```',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/cli-uasset-dump',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `uasset_dump-0.0.4/PKG-INFO` & `uasset_dump-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: uasset-dump
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure
 Home-page: https://github.com/bootloader-studio/cli-uasset-dump
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: cli,tool,utility,unreal,engine,asset,inventory,dump,json
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: perseus-core-library (>=1.19.2,<2.0.0)
+Requires-Dist: perseus-core-library (>=1.19.3,<2.0.0)
 Project-URL: Repository, https://github.com/bootloader-studio/cli-uasset-dump
 Description-Content-Type: text/markdown
 
 # Unreal Engine Assets Dump
 
 Command-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure.
 
@@ -124,9 +125,17 @@
   },
   (...)
 ]
 ```
 
 ```shell
 export UNREAL_ENGINE_PROJECT_PATH=/Users/admin/Library/JenkinsAgent/workspace/client-app/scooby-app-build/main/Scooby/Scooby.uproject
-`\"(find "/Users/Shared/Epic Games/UE_5.1" -name "UnrealEditor-Cmd")\"` "$UNREAL_ENGINE_PROJECT_PATH" -ExecutePythonScript="run.py"
+
+"`find "/Users/Shared/Epic Games/UE_5.2" -name UnrealEditor-Cmd`" \
+    "$UNREAL_ENGINE_PROJECT_PATH" \
+    -run=pythonscript \
+    -stdout \
+    -Unattended \
+    -script="/Users/admin/Downloads/run.py"
+
+echo $?;
 ```
```

