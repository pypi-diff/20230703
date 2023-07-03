# Comparing `tmp/uasset_dump-0.0.3.tar.gz` & `tmp/uasset_dump-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uasset_dump-0.0.3.tar", max compression
+gzip compressed data, was "uasset_dump-0.0.4.tar", max compression
```

## Comparing `uasset_dump-0.0.3.tar` & `uasset_dump-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      306 2023-03-31 11:18:04.579115 uasset_dump-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 uasset_dump-0.0.3/LICENSE.md
--rw-r--r--   0        0        0      989 2023-04-06 08:39:51.410335 uasset_dump-0.0.3/README.md
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.3/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.3/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.3/bootloader/ue/cli/__init__.py
--rwxr-xr-x   0        0        0     2445 2023-04-06 03:55:38.985331 uasset_dump-0.0.3/bootloader/ue/cli/uassetdump.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.3/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0     4797 2023-04-05 15:31:25.693554 uasset_dump-0.0.3/bootloader/ue/constant/uasset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.3/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0     2915 2023-04-05 14:09:09.558252 uasset_dump-0.0.3/bootloader/ue/model/uasset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.3/bootloader/ue/utils/__init__.py
--rw-r--r--   0        0        0     3917 2023-04-06 08:45:02.183427 uasset_dump-0.0.3/bootloader/ue/utils/uasset_dump.py
--rw-r--r--   0        0        0     1024 2023-04-06 08:45:15.951532 uasset_dump-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 uasset_dump-0.0.3/setup.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 uasset_dump-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-07-03 08:19:28.005425 uasset_dump-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 uasset_dump-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     3876 2023-07-03 07:33:54.680171 uasset_dump-0.0.4/README.md
+-rw-r--r--   0        0        0     1039 2023-07-03 08:23:51.764851 uasset_dump-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/ue/cli/__init__.py
+-rwxr-xr-x   0        0        0     2616 2023-07-03 08:21:18.490361 uasset_dump-0.0.4/src/bootloader/ue/cli/uassetdump.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.4/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0     4797 2023-04-05 15:31:25.693554 uasset_dump-0.0.4/src/bootloader/ue/constant/uasset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 uasset_dump-0.0.4/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0     2914 2023-06-14 02:27:45.682247 uasset_dump-0.0.4/src/bootloader/ue/model/uasset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 uasset_dump-0.0.4/src/bootloader/ue/utils/__init__.py
+-rw-r--r--   0        0        0     5496 2023-07-03 08:21:18.479007 uasset_dump-0.0.4/src/bootloader/ue/utils/uasset_dump.py
+-rw-r--r--   0        0        0     5079 1970-01-01 00:00:00.000000 uasset_dump-0.0.4/setup.py
+-rw-r--r--   0        0        0     4899 1970-01-01 00:00:00.000000 uasset_dump-0.0.4/PKG-INFO
```

### Comparing `uasset_dump-0.0.3/LICENSE.md` & `uasset_dump-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/__init__.py` & `uasset_dump-0.0.4/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/__init__.py` & `uasset_dump-0.0.4/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/cli/__init__.py` & `uasset_dump-0.0.4/src/bootloader/ue/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/cli/uassetdump.py` & `uasset_dump-0.0.4/src/bootloader/ue/cli/uassetdump.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,37 +12,38 @@
 # BOOTLOADER MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE
 # SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT
 # NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR
 # A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE
 # LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF
 # USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
 
-from pathlib import Path
 import argparse
+import sys
+from pathlib import Path
 
 from majormode.perseus.constant.logging import LOGGING_LEVEL_LITERAL_STRINGS
 from majormode.perseus.constant.logging import LoggingLevelLiteral
 from majormode.perseus.utils.logging import DEFAULT_LOGGING_FORMATTER
 from majormode.perseus.utils.logging import cast_string_to_logging_level
 from majormode.perseus.utils.logging import set_up_logger
 
-from bootloader.ue.utils import uasset_dump
+from src.bootloader.ue.utils import uasset_dump
 
 
 def cast_string_to_path(path: str) -> Path:
     return Path(path)
 
 
 def parse_arguments() -> argparse.Namespace:
     """
     Convert argument strings to objects and assign them as attributes of
     the namespace.
 
 
-    @return: An instance `Namespace` corresponding to the populated
+    :return: An object ``Namespace`` corresponding to the populated
         namespace.
     """
     parser = argparse.ArgumentParser(description="Unreal Engine project's asset list dump")
 
     parser.add_argument(
         '--logging-level',
         dest='logging_level',
@@ -65,8 +66,13 @@
     return parser.parse_args()
 
 
 def run():
     arguments = parse_arguments()
 
     set_up_logger(logging_formatter=DEFAULT_LOGGING_FORMATTER, logging_level=arguments.logging_level)
-    uasset_dump.dump_assets(arguments.path)
+
+    from timeit import default_timer as timer
+    start = timer()
+    print(uasset_dump.dump_assets(arguments.path))
+    end = timer()
+    sys.stderr.write(f"Asset dump completed in {end - start}s")
```

### Comparing `uasset_dump-0.0.3/bootloader/ue/constant/__init__.py` & `uasset_dump-0.0.4/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/constant/uasset.py` & `uasset_dump-0.0.4/src/bootloader/ue/constant/uasset.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/model/__init__.py` & `uasset_dump-0.0.4/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/model/uasset.py` & `uasset_dump-0.0.4/src/bootloader/ue/model/uasset.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 # BOOTLOADER MAKES NO REPRESENTATIONS OR WARRANTIES ABOUT THE
 # SUITABILITY OF THE SOFTWARE, EITHER EXPRESS OR IMPLIED, INCLUDING BUT
 # NOT LIMITED TO THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR
 # A PARTICULAR PURPOSE, OR NON-INFRINGEMENT.  BOOTLOADER SHALL NOT BE
 # LIABLE FOR ANY LOSSES OR DAMAGES SUFFERED BY LICENSEE AS A RESULT OF
 # USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
 
-
 class UAsset:
     def __init__(
             self,
             asset_name: str,
             asset_class_path: str,
             package_name: str,
             dependencies: list[str] or None):
         """
         Build a new {@link UAsset}.
 
 
-        @param asset_name: The name of the asset without the package.
+        :param asset_name: The name of the asset without the package.
 
-        @param asset_class_path: The path name of the asset’s class.
+        :param asset_class_path: The path name of the asset’s class.
 
-        @param package_name: The name of the package in which the asset is
+        :param package_name: The name of the package in which the asset is
             found.
 
-        @param dependencies: The list of names of the packages that the asset
+        :param dependencies: The list of names of the packages that the asset
             depends on.
         """
         self.__asset_name = asset_name
         self.__asset_class_path = asset_class_path
         self.__package_name = package_name
         self.__dependencies = dependencies
 
@@ -49,35 +48,35 @@
 
         ```text
         /Script/Engine/SkeletalMesh
         /Script/Engine/Skeleton
         /Script/Engine/Texture2D
         ```
 
-        @return: The path name of the asset's class.
+        :return: The path name of the asset's class.
         """
         return self.__asset_class_path
 
     @property
     def asset_name(self) -> str:
         """
         Return the name of the asset.
 
 
-        @return: The name of the asset without the package.
+        :return: The name of the asset without the package.
         """
         return self.__asset_name
 
     @property
     def dependencies(self) -> list[str] or None:
         """
         Return the list of names of the packages that the asset depends on.
 
 
-        @return: The list of names of the packages that the asset depends on.
+        :return: The list of names of the packages that the asset depends on.
         """
         return self.__dependencies
 
     def to_json(self) -> any:
         return {
             "asset_name": self.__asset_name,
             "asset_class_path": self.__asset_class_path,
@@ -87,10 +86,10 @@
 
     @property
     def package_name(self) -> str:
         """
         Return the name of the package in which the asset is found.
 
 
-        @return: The name of the package in which the asset is found.
+        :return: The name of the package in which the asset is found.
         """
         return self.__package_name
```

### Comparing `uasset_dump-0.0.3/bootloader/ue/utils/__init__.py` & `uasset_dump-0.0.4/src/bootloader/ue/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `uasset_dump-0.0.3/bootloader/ue/utils/uasset_dump.py` & `uasset_dump-0.0.4/src/bootloader/ue/utils/uasset_dump.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,60 +14,30 @@
 # USING, MODIFYING OR DISTRIBUTING THIS SOFTWARE OR ITS DERIVATIVES.
 
 import json
 from pathlib import Path
 
 import unreal
 
-from bootloader.ue.model.uasset import UAsset
+from src.bootloader.ue.model.uasset import UAsset
 
 
 UNREAL_ENGINE_PROJECT_CONTENT_PATH = '/Game/'
 
 
-def dump_assets(root_path: str or Path) -> None:
-    assets = find_assets(root_path)
-    print(json.dumps([asset.to_json() for asset in assets], indent=2))
-
-
-def find_assets(content_path: str) -> list[UAsset]:
-    """
-    Return the list of the assets found recursively in the specified path.
-
-
-    @param content_path: The path to the assets.
-
-
-    @return: The list of the assets found in the specified path.
-    """
-    # Retrieve the list of the paths of the assets found recursively in the
-    # specified path.
-    asset_paths = unreal.EditorAssetLibrary.list_assets(content_path, True, False)
-
-    # Build the list of assets.
-    assets = []
-
-    for asset_path in asset_paths:
-        asset_data = unreal.EditorAssetLibrary.find_asset_data(asset_path)
-        if asset_data.is_valid() and asset_data.is_u_asset():  # @note: Usually always true, but who knows?...
-            assets.append(get_asset(asset_data))
-
-    return assets
-
-
-def get_asset(asset_data: unreal.AssetData) -> UAsset:
+def build_asset(asset_data: unreal.AssetData) -> UAsset:
     """
     Return an instance {@link UAsset} from the asset data.
 
 
-    @param asset_data: The data of the asset returned by the Unreal Engine
+    :param asset_data: The data of the asset returned by the Unreal Engine
         Python API's Asset Registry.
 
 
-    @return: An instance {@link UAsset}.
+    :return: An instance {@link UAsset}.
     """
     asset_name = asset_data.asset_name
     package_name = asset_data.package_name
 
     # @note: The property `asset_class` has been deprecated.  The asset
     #     class name must be converted to full asset pathname.
     asset_class = f'{asset_data.asset_class_path.package_name}/{asset_data.asset_class_path.asset_name}'
@@ -82,28 +52,44 @@
         str(package_name),
         dependencies
     )
 
     return asset
 
 
+def dump_assets(root_path: str or Path) -> str:
+    """
+    Serialize the assets found in the specified path to JSON formatted
+    string.
+
+
+    :param root_path: The path to the assets.
+
+
+    :return: A JSON string representing the list of assets.
+    """
+    assets = find_assets(root_path)
+    json_string = json.dumps([asset.to_json() for asset in assets], indent=2)
+    return json_string
+
+
 def find_asset_dependencies(asset_data: unreal.DataAsset):
     """
     Return the list of the package names of assets that the specified
     asset depends on.
 
     The function excludes any Unreal Engine's assets.  The function only
     includes assets from the game itself.
 
 
-    @param asset_data: The data of the asset returned by the Unreal Engine
+    :param asset_data: The data of the asset returned by the Unreal Engine
         Python API's Asset Registry.
 
 
-    @return: A list of the package names of assets.
+    :return: A list of the package names of assets.
     """
     asset_registry = unreal.AssetRegistryHelpers.get_asset_registry()
     dependency_options = unreal.AssetRegistryDependencyOptions(
         # include_soft_package_references=True,
         # include_hard_package_references=True,
         # include_searchable_names=True,
         # include_soft_management_references=True,
@@ -113,7 +99,78 @@
     asset_dependencies_package_name = asset_registry.get_dependencies(asset_data.package_name, dependency_options)
 
     return [
         str(package_name)
         for package_name in asset_dependencies_package_name
         if str(package_name).startswith(UNREAL_ENGINE_PROJECT_CONTENT_PATH)
     ]
+
+
+def find_assets(content_path: str) -> list[UAsset]:
+    """
+    Return the list of the assets found recursively in the specified path.
+
+
+    :param content_path: The path to the assets.
+
+
+    :return: The list of the assets found in the specified path.
+    """
+    # Retrieve the list of the paths of the assets found recursively in the
+    # specified path.
+    asset_paths: list = unreal.EditorAssetLibrary.list_assets(content_path, True, False)
+
+    # Build the list of assets.
+    #
+    # @note: Using list comprehension if faster than `loop` (indeed!):
+    #
+    #     ```python
+    #     assets = []
+    #     assets_append = assets.append
+    #     for asset_path in asset_paths:
+    #         asset_data = unreal.EditorAssetLibrary.find_asset_data(asset_path)
+    #         if asset_data.is_valid() and asset_data.is_u_asset():  # @note: Usually always true, but who knows?...
+    #             assets_append(build_asset(asset_data))
+    #     ```
+    #
+    #     And faster than `map` when not using a `lambda`:
+    #
+    #     ```python
+    #     assets = list(
+    #         filter(
+    #             lambda asset: asset is not None,
+    #             map(get_asset, asset_paths)
+    #         )
+    #     )
+    #     ```
+    #
+    #   Result with 1k assets:
+    #
+    #   - Loop --> 0.6712107429998468
+    #   - List comprehension --> 0.05552284200030044
+    #   - Map --> 0.20423201099993094
+    assets = [
+        build_asset(asset_data)
+        for asset_data in [
+            unreal.EditorAssetLibrary.find_asset_data(asset_path)
+            for asset_path in asset_paths
+        ]
+        if asset_data.is_valid() and asset_data.is_u_asset()
+    ]
+
+    return assets
+
+
+def get_asset(asset_path):
+    """
+    Return the data of the specified asset.
+
+
+    :param asset_path: The Unreal Engine path of the asset.
+
+
+    :return: The asset's data if the asset is valid and is an Unreal
+        Engine asset; ``None`` otherwise.
+    """
+    asset_data = unreal.EditorAssetLibrary.find_asset_data(asset_path)
+    if asset_data.is_valid() and asset_data.is_u_asset():
+        return build_asset(asset_data)
```

### Comparing `uasset_dump-0.0.3/pyproject.toml` & `uasset_dump-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 description = "Command-line Interface (CLI) responsible for returning the list of the assets of an Unreal Engine project into a JSON structure"
 include = [
     "CHANGELOG.md",
 ]
 keywords = ["cli", "tool", "utility", "unreal", "engine", "asset", "inventory", "dump", "json"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "uasset-dump"
-packages = [{ include = "bootloader" }]
+packages = [{ include = "bootloader", from = "src" }]
 readme = "README.md"
 repository = "https://github.com/bootloader-studio/cli-uasset-dump"
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.2"
-python = "^3.9"
+python = "^3.10"
 
 [tool.poetry.scripts]
 ueprjver = 'bootloader.ue.cli.uassetdump:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

