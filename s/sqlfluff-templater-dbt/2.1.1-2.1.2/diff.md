# Comparing `tmp/sqlfluff-templater-dbt-2.1.1.tar.gz` & `tmp/sqlfluff-templater-dbt-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-j4b_a0t4/sqlfluff-templater-dbt-2.1.1.tar", last modified: Thu May 25 16:29:33 2023, max compression
+gzip compressed data, was "/home/runner/work/sqlfluff/sqlfluff/plugins/sqlfluff-templater-dbt/dist/.tmp-k_7h5azy/sqlfluff-templater-dbt-2.1.2.tar", last modified: Mon Jul  3 08:40:06 2023, max compression
```

## Comparing `sqlfluff-templater-dbt-2.1.1.tar` & `sqlfluff-templater-dbt-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25159 2023-05-25 16:29:15.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 16:29:33.000000 sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-03 08:39:47.000000 sqlfluff-templater-dbt-2.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 08:39:47.000000 sqlfluff-templater-dbt-2.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 08:39:47.000000 sqlfluff-templater-dbt-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-03 08:39:47.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-07-03 08:39:47.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-03 08:40:06.000000 sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/top_level.txt
```

### Comparing `sqlfluff-templater-dbt-2.1.1/LICENSE.md` & `sqlfluff-templater-dbt-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-templater-dbt-2.1.1/PKG-INFO` & `sqlfluff-templater-dbt-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.1.1
+Version: 2.1.2
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

### Comparing `sqlfluff-templater-dbt-2.1.1/setup.cfg` & `sqlfluff-templater-dbt-2.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlfluff-templater-dbt
-version = 2.1.1
+version = 2.1.2
 description = Lint your dbt project SQL
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sqlfluff/sqlfluff
 author = Alan Cruickshank
 author_email = alan@designingoverload.com
 license = MIT License
@@ -61,15 +61,15 @@
 	tsql
 	dbt
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	sqlfluff==2.1.1
+	sqlfluff==2.1.2
 	dbt-core>=1.0.0
 	jinja2-simple-tags>=0.3.1
 	markupsafe
 	pydantic
 	rich
 	ruamel.yaml
```

### Comparing `sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt/templater.py` & `sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt/templater.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,40 @@
 """Defines the templaters."""
 
 from collections import deque
 from contextlib import contextmanager
 import os
 import os.path
 import logging
-from typing import List, Optional, Iterator, Tuple, Any, Dict, Deque
+from typing import List, Optional, Iterator, Tuple, Any, Dict, Deque, Union
 
 from dataclasses import dataclass
 
 from dbt.version import get_installed_version
+from dbt.config import read_user_config
 from dbt.config.runtime import RuntimeConfig as DbtRuntimeConfig
 from dbt.adapters.factory import register_adapter, get_adapter
 from dbt.compilation import Compiler as DbtCompiler
-from dbt.cli.resolvers import default_profiles_dir
+
+# From dbt 1.3 onwards, the default_profiles_dir resolver is
+# available. Before that version we use the flags module
+try:
+    from dbt.cli.resolvers import default_profiles_dir
+except ImportError:
+    default_profiles_dir = None
+
+# After this PR on dbt-core, we need to inject context variables
+# directly. This change was backported and so exists in some versions
+# but not others. When not present, no additional action is needed.
+# https://github.com/dbt-labs/dbt-core/pull/7949
+# On the 1.5.x branch this was between 1.5.1 and 1.5.2
+try:
+    from dbt.task.contextvars import cv_project_root
+except ImportError:
+    cv_project_root = None
 
 try:
     from dbt.exceptions import (
         CompilationException as DbtCompilationException,
         FailedToConnectException as DbtFailedToConnectException,
         DbtProjectError,
     )
@@ -63,15 +80,16 @@
 
     project_dir: Optional[str] = None
     profiles_dir: Optional[str] = None
     profile: Optional[str] = None
     target: Optional[str] = None
     threads: int = 1
     single_threaded: bool = False
-    vars: Optional[Dict] = None
+    # dict in 1.5.x onwards, json string before.
+    vars: Optional[Union[Dict, str]] = None if DBT_VERSION_TUPLE >= (1, 5) else ""
 
 
 class DbtTemplater(JinjaTemplater):
     """A templater using dbt."""
 
     name = "dbt"
     sequential_fail_limit = 3
@@ -94,31 +112,46 @@
     def dbt_version(self):  # pragma: no cover
         """Gets the dbt version."""
         return DBT_VERSION_STRING
 
     @cached_property
     def dbt_config(self):
         """Loads the dbt config."""
+        if DBT_VERSION_TUPLE >= (1, 5):
+            user_config = None
+            # 1.5.x+ this is a dict.
+            cli_vars = self._get_cli_vars()
+        else:
+            # Here, we read flags.PROFILE_DIR directly, prior to calling
+            # set_from_args(). Apparently, set_from_args() sets PROFILES_DIR
+            # to a lowercase version of the value, and the profile wouldn't be
+            # found if the directory name contained uppercase letters. This fix
+            # was suggested and described here:
+            # https://github.com/sqlfluff/sqlfluff/issues/2253#issuecomment-1018722979
+            user_config = read_user_config(flags.PROFILES_DIR)
+            # Pre 1.5.x this is a string.
+            cli_vars = str(self._get_cli_vars())
+
         flags.set_from_args(
             DbtConfigArgs(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 profile=self._get_profile(),
-                vars=self._get_cli_vars(),
+                vars=cli_vars,
                 threads=1,
             ),
-            None,
+            user_config,
         )
         self.dbt_config = DbtRuntimeConfig.from_args(
             DbtConfigArgs(
                 project_dir=self.project_dir,
                 profiles_dir=self.profiles_dir,
                 profile=self._get_profile(),
                 target=self._get_target(),
-                vars=self._get_cli_vars(),
+                vars=cli_vars,
                 threads=1,
             )
         )
         register_adapter(self.dbt_config)
         return self.dbt_config
 
     @cached_property
@@ -141,20 +174,25 @@
         from dbt.parser.manifest import ManifestLoader
 
         old_cwd = os.getcwd()
         try:
             # Changing cwd temporarily as dbt is not using project_dir to
             # read/write `target/partial_parse.msgpack`. This can be undone when
             # https://github.com/dbt-labs/dbt-core/issues/6055 is solved.
-            os.chdir(self.project_dir)
+            # For dbt 1.4+ this isn't necessary, but it is required for 1.3
+            # and before.
+            if DBT_VERSION_TUPLE < (1, 4):
+                os.chdir(self.project_dir)
             self.dbt_manifest = ManifestLoader.get_full_manifest(self.dbt_config)
         except DbtProjectError as err:  # pragma: no cover
             raise SQLFluffUserError(f"DbtProjectError: {err}")
         finally:
-            os.chdir(old_cwd)
+            if DBT_VERSION_TUPLE < (1, 4):
+                os.chdir(old_cwd)
+
         return self.dbt_manifest
 
     @cached_property
     def dbt_selector_method(self):
         """Loads the dbt selector method."""
         if self.formatter:  # pragma: no cover TODO?
             self.formatter.dispatch_compilation_header(
@@ -185,20 +223,29 @@
 
         The default is `~/.dbt` but we use the
         default_profiles_dir from the dbt library to
         support a change of default in the future, as well
         as to support the same overwriting mechanism as
         dbt (currently an environment variable).
         """
+        # Where default_profiles_dir is available, use it. For dbt 1.2 and
+        # earlier, it is not, so fall back to the flags option which should
+        # still be available in those versions.
+        default_dir = (
+            default_profiles_dir()
+            if default_profiles_dir is not None
+            else flags.PROFILES_DIR
+        )
+
         dbt_profiles_dir = os.path.abspath(
             os.path.expanduser(
                 self.sqlfluff_config.get_section(
                     (self.templater_selector, self.name, "profiles_dir")
                 )
-                or (os.getenv("DBT_PROFILES_DIR") or default_profiles_dir())
+                or (os.getenv("DBT_PROFILES_DIR") or default_dir)
             )
         )
 
         if not os.path.exists(dbt_profiles_dir):
             templater_logger.error(
                 f"dbt_profiles_dir: {dbt_profiles_dir} could not be accessed. "
                 "Check it exists."
@@ -460,14 +507,20 @@
 
                         def make_template(in_str):
                             env.add_extension(SnapshotExtension)
                             return env.from_string(in_str, globals=globals)
 
             return old_from_string(*args, **kwargs)
 
+        # NOTE: We need to inject the project root here in reaction to the
+        # breaking change upstream with dbt.
+        # https://github.com/dbt-labs/dbt-core/pull/7949
+        if cv_project_root is not None:
+            cv_project_root.set(self.project_dir)
+
         node = self._find_node(fname, config)
         templater_logger.debug(
             "_find_node for path %r returned object of type %s.", fname, type(node)
         )
 
         save_ephemeral_nodes = dict(
             (k, v)
```

### Comparing `sqlfluff-templater-dbt-2.1.1/sqlfluff_templater_dbt.egg-info/PKG-INFO` & `sqlfluff-templater-dbt-2.1.2/sqlfluff_templater_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff-templater-dbt
-Version: 2.1.1
+Version: 2.1.2
 Summary: Lint your dbt project SQL
 Home-page: https://github.com/sqlfluff/sqlfluff
 Author: Alan Cruickshank
 Author-email: alan@designingoverload.com
 License: MIT License
 Project-URL: Homepage, https://www.sqlfluff.com
 Project-URL: Documentation, https://docs.sqlfluff.com
```

