# Comparing `tmp/delfino_core-5.1.1.tar.gz` & `tmp/delfino_core-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino_core-5.1.1.tar", max compression
+gzip compressed data, was "delfino_core-5.2.0.tar", max compression
```

## Comparing `delfino_core-5.1.1.tar` & `delfino_core-5.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1078 2023-06-25 13:19:48.163020 delfino_core-5.1.1/LICENSE.md
--rw-r--r--   0        0        0     5291 2023-06-25 13:19:48.163020 delfino_core-5.1.1/README.md
--rw-r--r--   0        0        0     4246 2023-06-25 13:19:48.163020 delfino_core-5.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/__init__.py
--rw-r--r--   0        0        0      293 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/backports.py
--rw-r--r--   0        0        0        0 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/__init__.py
--rw-r--r--   0        0        0     9018 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/dependencies_update.py
--rw-r--r--   0        0        0     4416 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/format.py
--rw-r--r--   0        0        0     6812 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/lint.py
--rw-r--r--   0        0        0     3471 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/switch_python_version.py
--rw-r--r--   0        0        0     7858 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/test.py
--rw-r--r--   0        0        0     3446 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/commands/typecheck.py
--rw-r--r--   0        0        0      748 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/commands/verify_all.py
--rw-r--r--   0        0        0      904 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/config.py
--rw-r--r--   0        0        0     1720 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/utils.py
--rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 delfino_core-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-03 09:12:34.393504 delfino_core-5.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5291 2023-07-03 09:12:34.393504 delfino_core-5.2.0/README.md
+-rw-r--r--   0        0        0     4246 2023-07-03 09:12:34.393504 delfino_core-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/__init__.py
+-rw-r--r--   0        0        0      293 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/backports.py
+-rw-r--r--   0        0        0        0 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/__init__.py
+-rw-r--r--   0        0        0     9368 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/dependencies_update.py
+-rw-r--r--   0        0        0     4416 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/format.py
+-rw-r--r--   0        0        0     6812 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/lint.py
+-rw-r--r--   0        0        0     3471 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/switch_python_version.py
+-rw-r--r--   0        0        0     7858 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/test.py
+-rw-r--r--   0        0        0     3446 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/typecheck.py
+-rw-r--r--   0        0        0      748 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/commands/verify_all.py
+-rw-r--r--   0        0        0      904 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/config.py
+-rw-r--r--   0        0        0     1720 2023-07-03 09:12:34.393504 delfino_core-5.2.0/src/delfino_core/utils.py
+-rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 delfino_core-5.2.0/PKG-INFO
```

### Comparing `delfino_core-5.1.1/LICENSE.md` & `delfino_core-5.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/README.md` & `delfino_core-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/pyproject.toml` & `delfino_core-5.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="delfino-core"
-version="5.1.1"
+version="5.2.0"
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 description="Delfino core plugin"
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino-core"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/dependencies_update.py` & `delfino_core-5.2.0/src/delfino_core/commands/dependencies_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,19 @@
     def _git_root():
         return (
             run(["git", "rev-parse", "--show-toplevel"], capture_output=True, on_error=OnError.EXIT)
             .stdout.decode()
             .strip()
         )
 
-    def __init__(self):
+    def __init__(self, stash: bool):
         assert_pip_package_installed("gitpython")
 
         self._repo = Repo(self._git_root())
+        self._stash = stash
         now = datetime.utcnow()
         self._start_of_week = now - timedelta(now.isoweekday() - 1)
 
     def commit_and_push(self):
         commit_message = f"Dependencies rollup: {self._start_of_week.strftime('%Y-%m-%d')}"
         can_update = self._repo.commit("HEAD").message.strip() == commit_message
 
@@ -119,16 +120,17 @@
     def checkout_branch(self, branch: str):
         if str(self._repo.active_branch) == branch:
             secho(f"Branch '{branch}' already exists and active.", fg="green")
         elif branch in self._repo.branches:  # type: ignore[operator]
             secho(f"Branch '{branch}' already exists.", fg="yellow")
             _run(f"git checkout {branch}")
         else:
-            secho("Stashing existing changes.", fg="yellow")
-            _run("git stash")
+            if self._stash:
+                secho("Stashing existing changes.", fg="yellow")
+                _run("git stash")
 
             if self._repo.active_branch != "main":
                 secho("Checking out 'main'.", fg="yellow")
                 _run("git checkout main")
 
             secho("Pulling latest changes.", fg="yellow")
             _run("git pull")
@@ -214,28 +216,37 @@
 
         self._show_edit_prompt_and_wait(available_updates=result.stdout.decode())
 
         return self._read_dependency_file() != pyproject_toml
 
 
 @click.command()
-@click.option("--retry", default=False, show_default=True, is_flag=True, help=" Retry an update after failed tests.")
+@click.option("--retry", default=False, show_default=True, is_flag=True, help="Retry an update after failed tests.")
+@click.option(
+    "--stash/--no-stash",
+    default=True,
+    show_default=True,
+    help=(
+        "Don't stash existing changes. Useful when there are some existing manual changes "
+        "that should be also part of the upgrade."
+    ),
+)
 @pass_app_context(CorePluginConfig)
 @click.pass_context
-def dependencies_update(click_context: click.Context, app_context: AppContext, retry):
+def dependencies_update(click_context: click.Context, app_context: AppContext, retry: bool, stash: bool):
     """Manages the process of updating dependencies."""
     print_header("Updating dependencies", icon="🔄")
 
     assert_package_manager_is_known(app_context.package_manager)
     updater: Updater
 
     if app_context.package_manager == PackageManager.PIPENV:
-        updater = PipenvUpdater()
+        updater = PipenvUpdater(stash)
     elif app_context.package_manager == PackageManager.POETRY:
-        updater = PoetryUpdater()
+        updater = PoetryUpdater(stash)
     else:
         raise AssertionError(
             f"The '{app_context.package_manager.value}' package manager is not supported by this command."
         )
 
     updater.update(retry)
```

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/format.py` & `delfino_core-5.2.0/src/delfino_core/commands/format.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/lint.py` & `delfino_core-5.2.0/src/delfino_core/commands/lint.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/switch_python_version.py` & `delfino_core-5.2.0/src/delfino_core/commands/switch_python_version.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/test.py` & `delfino_core-5.2.0/src/delfino_core/commands/test.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/typecheck.py` & `delfino_core-5.2.0/src/delfino_core/commands/typecheck.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/commands/verify_all.py` & `delfino_core-5.2.0/src/delfino_core/commands/verify_all.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/config.py` & `delfino_core-5.2.0/src/delfino_core/config.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/src/delfino_core/utils.py` & `delfino_core-5.2.0/src/delfino_core/utils.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.1/PKG-INFO` & `delfino_core-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delfino-core
-Version: 5.1.1
+Version: 5.2.0
 Summary: Delfino core plugin
 Home-page: https://github.com/radeklat/delfino-core
 License: MIT
 Author: Radek Lát
 Author-email: radek.lat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: delfino-core Version: 5.1.1 Summary: Delfino core
+Metadata-Version: 2.1 Name: delfino-core Version: 5.2.0 Summary: Delfino core
 plugin Home-page: https://github.com/radeklat/delfino-core License: MIT Author:
 Radek LÃ¡t Author-email: radek.lat@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

