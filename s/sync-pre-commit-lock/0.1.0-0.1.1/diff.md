# Comparing `tmp/sync_pre_commit_lock-0.1.0.tar.gz` & `tmp/sync_pre_commit_lock-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sync_pre_commit_lock-0.1.0.tar", last modified: Sun Jul  2 18:51:09 2023, max compression
+gzip compressed data, was "sync_pre_commit_lock-0.1.1.tar", last modified: Mon Jul  3 18:30:02 2023, max compression
```

## Comparing `sync_pre_commit_lock-0.1.0.tar` & `sync_pre_commit_lock-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/LICENSE
--rw-r--r--   0        0        0     3364 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/README.md
--rw-r--r--   0        0        0     2819 2023-07-02 18:51:09.838910 sync_pre_commit_lock-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      908 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/actions/__init__.py
--rw-r--r--   0        0        0     3151 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/actions/install_hooks.py
--rw-r--r--   0        0        0     8276 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/actions/sync_hooks.py
--rw-r--r--   0        0        0     1960 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/config.py
--rw-r--r--   0        0        0     1694 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/db.py
--rw-r--r--   0        0        0     3607 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/pdm_plugin.py
--rw-r--r--   0        0        0     4236 2023-07-02 18:50:54.322971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/poetry_plugin.py
--rw-r--r--   0        0        0       93 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/py.typed
--rw-r--r--   0        0        0     1203 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/utils.py
--rw-r--r--   0        0        0       39 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      405 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/fixtures/poetry_project/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8012 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/fixtures/poetry_project/poetry.lock
--rw-r--r--   0        0        0      412 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/fixtures/poetry_project/pyproject.toml
--rw-r--r--   0        0        0     6401 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_actions/test_install_hooks.py
--rw-r--r--   0        0        0     5985 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_actions/test_pre_commit_config_file.py
--rw-r--r--   0        0        0    13291 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_actions/test_sync_hooks.py
--rw-r--r--   0        0        0     2576 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_config.py
--rw-r--r--   0        0        0      273 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_db.py
--rw-r--r--   0        0        0     3146 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_pdm/test_pdm_plugin.py
--rw-r--r--   0        0        0     2045 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_pdm/test_pdm_sync_pre_commit_hook.py
--rw-r--r--   0        0        0     3192 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_poetry/test_poetry_plugin.py
--rw-r--r--   0        0        0     1323 2023-07-02 18:50:54.326971 sync_pre_commit_lock-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0    45168 1970-01-01 00:00:00.000000 sync_pre_commit_lock-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-03 18:29:44.407432 sync_pre_commit_lock-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4926 2023-07-03 18:29:44.407432 sync_pre_commit_lock-0.1.1/README.md
+-rw-r--r--   0        0        0     2880 2023-07-03 18:30:02.983523 sync_pre_commit_lock-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      908 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/actions/__init__.py
+-rw-r--r--   0        0        0     3199 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/actions/install_hooks.py
+-rw-r--r--   0        0        0     8272 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/actions/sync_hooks.py
+-rw-r--r--   0        0        0     2039 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/config.py
+-rw-r--r--   0        0        0     1694 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/db.py
+-rw-r--r--   0        0        0     3586 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/pdm_plugin.py
+-rw-r--r--   0        0        0     4157 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/poetry_plugin.py
+-rw-r--r--   0        0        0       93 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/py.typed
+-rw-r--r--   0        0        0     1172 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/utils.py
+-rw-r--r--   0        0        0       39 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      405 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/fixtures/poetry_project/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8012 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/fixtures/poetry_project/poetry.lock
+-rw-r--r--   0        0        0      412 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/fixtures/poetry_project/pyproject.toml
+-rw-r--r--   0        0        0     6401 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_actions/test_install_hooks.py
+-rw-r--r--   0        0        0     6031 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_actions/test_pre_commit_config_file.py
+-rw-r--r--   0        0        0    13291 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_actions/test_sync_hooks.py
+-rw-r--r--   0        0        0     2736 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_config.py
+-rw-r--r--   0        0        0      273 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_db.py
+-rw-r--r--   0        0        0     3156 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_pdm/test_pdm_plugin.py
+-rw-r--r--   0        0        0     2045 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_pdm/test_pdm_sync_pre_commit_hook.py
+-rw-r--r--   0        0        0     3192 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_poetry/test_poetry_plugin.py
+-rw-r--r--   0        0        0     1323 2023-07-03 18:29:44.411432 sync_pre_commit_lock-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0    46730 1970-01-01 00:00:00.000000 sync_pre_commit_lock-0.1.1/PKG-INFO
```

### Comparing `sync_pre_commit_lock-0.1.0/LICENSE` & `sync_pre_commit_lock-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/pyproject.toml` & `sync_pre_commit_lock-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "sync-pre-commit-lock"
-version = "0.1.0"
+version = "0.1.1"
 description = "PDM plugin to sync your pre-commit versions with your lockfile."
 authors = [
     { name = "Gabriel Dugny", email = "sync-pre-commit-lock@dugny.me" },
 ]
 dependencies = [
     "PyYAML>=6.0",
     "tomli>=2.0.0; python_version < \"3.11\"",
@@ -73,14 +73,20 @@
 [tool.ruff]
 line-length = 140
 respect-gitignore = true
 extend-select = [
     "Q000",
     "TCH",
     "I001",
+    "S",
+    "T",
+    "PTH",
+]
+extend-ignore = [
+    "S101",
 ]
 target-version = "py310"
 
 [tool.mypy]
 strict = true
 
 [tool.black]
```

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/__init__.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/__init__.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/actions/install_hooks.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/actions/install_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         self._install_pre_commit_hooks()
 
     def _install_pre_commit_hooks(self) -> None:
         try:
             self.printer.info("Installing pre-commit hooks...")
             return_code = subprocess.check_call(
-                self.install_pre_commit_hooks_command,
+                self.install_pre_commit_hooks_command,  # noqa: S603
                 # XXX We probably want to see the output, at least in verbose mode or if it fails
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
             if return_code == 0:
                 self.printer.info("pre-commit hooks successfully installed!")
             else:
@@ -58,26 +58,26 @@
             self.printer.error("Failed to install pre-commit hooks due to an unexpected error")
             self.printer.error(f"{e}")
 
     def _is_pre_commit_package_installed(self) -> bool:
         try:
             # Try is `pre-commit --version` works
             output = subprocess.check_output(
-                self.check_pre_commit_version_command,
+                self.check_pre_commit_version_command,  # noqa: S603
             ).decode()
             return "pre-commit" in output
         except FileNotFoundError:
             return False
 
     @staticmethod
     def _are_pre_commit_hooks_installed(git_root: Path) -> bool:
         return (git_root / "hooks" / "pre-commit").exists()
 
     @staticmethod
     def _get_git_directory_path() -> Path | None:
         try:
             result = subprocess.check_output(
-                ["git", "rev-parse", "--show-toplevel"],
+                ["git", "rev-parse", "--show-toplevel"],  # noqa: S603, S607
             )
             return Path(result.decode().strip()) / ".git"
         except (subprocess.CalledProcessError, FileNotFoundError):
             return None
```

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/actions/sync_hooks.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/actions/sync_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         return [PreCommitRepo(repo=repo["repo"], rev=repo["rev"]) for repo in (self.data["repos"] or [])]
 
     @cached_property
     def repos_normalized(self) -> set[PreCommitRepo]:
         return {PreCommitRepo(repo=normalize_git_url(repo.repo), rev=repo.rev) for repo in self.repos}
 
     def update_pre_commit_repo_versions(self, new_versions: dict[PreCommitRepo, str]) -> None:
-        """Fixes the pre-commit hooks to match the lockfile. Preserves comments and formatting as much as possible."""
+        """Fix the pre-commit hooks to match the lockfile. Preserve comments and formatting as much as possible."""
 
         original_lines = self.original_file_lines
         updated_lines = original_lines[:]
         pre_commit_data = self.data
 
         for repo, rev in new_versions.items():
             for pre_commit_repo in pre_commit_data["repos"]:
@@ -78,15 +78,15 @@
                 updated_lines[rev_line_number] = re.sub(r"(?<=rev: )\S*", rev, original_rev_line)
 
         changes = difflib.ndiff(original_lines, updated_lines)
         change_count = sum(1 for change in changes if change[0] in ["+", "-"])
 
         if change_count == 0:
             return
-        with open(self.pre_commit_config_file_path, "w") as stream:
+        with self.pre_commit_config_file_path.open("w") as stream:
             stream.writelines(updated_lines)
 
 
 class SyncPreCommitHooksVersion:
     def __init__(
         self,
         printer: Printer,
```

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/config.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from pathlib import Path
 from typing import TYPE_CHECKING, Any, TypeVar
 
 try:
     # 3.11+
     import tomllib as toml  # type: ignore[import,unused-ignore]
 except ImportError:
     import tomli as toml  # type: ignore[no-redef,unused-ignore]
@@ -39,17 +40,18 @@
     automatically_install_hooks: bool = field(default=True, metadata={"toml": "automatically-install-hooks"})
     disable_sync_from_lock: bool = field(default=False, metadata={"toml": "disable-sync-from-lock"})
     ignore: list[str] = field(default_factory=list, metadata={"toml": "ignore"})
     pre_commit_config_file: str = field(metadata={"toml": "pre-commit-config-file"}, default=".pre-commit-config.yaml")
     dependency_mapping: PackageRepoMapping = field(default_factory=dict, metadata={"toml": "dependency-mapping"})
 
 
-def load_config() -> SyncPreCommitLockConfig:
-    # XXX We Should not harcode this, and get the filename from PDM/Poetry/custom resolution
-    with open("pyproject.toml", "rb") as file:
+def load_config(path: Path | None = None) -> SyncPreCommitLockConfig:
+    # XXX We Should not hardcode this, and get the filename from PDM/Poetry/custom resolution
+    path = path or Path("pyproject.toml")
+    with path.open("rb") as file:
         config_dict = toml.load(file)
 
     tool_dict = config_dict.get("tool", {}).get("sync-pre-commit-lock", {})
     if not tool_dict or len(tool_dict) == 0:
         return SyncPreCommitLockConfig()
 
     return from_toml(tool_dict)
```

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/db.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/db.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/pdm_plugin.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/pdm_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     printer.debug("Checking if pre-commit hooks are installed")
 
     if not plugin_config.automatically_install_hooks:
         printer.debug("Automatically installing pre-commit hooks is disabled. Skipping.")
         return None
     action = PDMSetupPreCommitHooks(printer, dry_run=dry_run)
     file_path = project.root / plugin_config.pre_commit_config_file
-    print(file_path)
     if not file_path.exists():
         printer.info("No pre-commit config file found, skipping pre-commit hook check")
         return None
 
     printer.debug("Pre-commit config file found. Setting up pre-commit hooks...")
 
     action.execute()
```

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/poetry_plugin.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/poetry_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import os
 from pathlib import Path
 from typing import TYPE_CHECKING, ClassVar
 
 from cleo.events.console_events import TERMINATE
 from cleo.events.console_terminate_event import ConsoleTerminateEvent
 from cleo.io.outputs.output import Verbosity
 from poetry.console.commands.add import AddCommand
@@ -59,16 +58,14 @@
         application.event_dispatcher.add_listener(TERMINATE, self._handle_post_command)
 
         self.application = application
 
     def _handle_post_command(
         self, event: ConsoleTerminateEvent | Event, event_name: str, dispatcher: EventDispatcher
     ) -> None:
-        print("SyncPreCommitLockPlugin handling post command")
-
         assert isinstance(event, ConsoleTerminateEvent)
         if event.exit_code != 0:
             # The command failed, so the plugin shouldn't do anything
             return
 
         command = event.command
         printer = PoetryPrinter(event.io)
@@ -87,15 +84,15 @@
 
             # Get all locked dependencies from self.application
             poetry_locked_packages = self.application.poetry.locker.locked_repository().packages
             locked_packages = {
                 str(p.name): GenericLockedPackage(p.name, str(p.version)) for p in poetry_locked_packages
             }
             plugin_config = load_config()
-            file_path = Path(os.getcwd()) / plugin_config.pre_commit_config_file
+            file_path = Path().cwd() / plugin_config.pre_commit_config_file
 
             SyncPreCommitHooksVersion(
                 printer,
                 pre_commit_config_file_path=file_path,
                 plugin_config=plugin_config,
                 locked_packages=locked_packages,
                 dry_run=dry_run,
```

### Comparing `sync_pre_commit_lock-0.1.0/src/sync_pre_commit_lock/utils.py` & `sync_pre_commit_lock-0.1.1/src/sync_pre_commit_lock/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,18 +14,15 @@
 
     # Normalize the scheme: convert git, git+ssh, and ssh to https
     scheme = parsed_url.scheme
     if scheme in ["git", "git+ssh", "ssh"]:
         scheme = "https"
 
     # Lowercase the hostname and remove default port if it exists
-    if parsed_url.hostname:
-        netloc = parsed_url.hostname.lower()
-    else:
-        netloc = ""
+    netloc = parsed_url.hostname.lower() if parsed_url.hostname else ""
 
     # If netloc is empty (git, ssh URLs), then path contains it.
     if not netloc:
         return url  # malformed URL, we can't normalize it
 
     path = parsed_url.path
```

### Comparing `sync_pre_commit_lock-0.1.0/tests/fixtures/poetry_project/poetry.lock` & `sync_pre_commit_lock-0.1.1/tests/fixtures/poetry_project/poetry.lock`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_actions/test_install_hooks.py` & `sync_pre_commit_lock-0.1.1/tests/test_actions/test_install_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_actions/test_pre_commit_config_file.py` & `sync_pre_commit_lock-0.1.1/tests/test_actions/test_pre_commit_config_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,26 +76,27 @@
 
 @patch("sync_pre_commit_lock.actions.sync_hooks.difflib")
 @patch("sync_pre_commit_lock.actions.sync_hooks.re")
 @patch("builtins.open", new_callable=mock_open)
 def test_update_pre_commit_repo_versions(mock_open_file: MagicMock, mock_re: MagicMock, mock_diff: MagicMock) -> None:
     data = {"repos": [{"repo": "repo1", "rev": "rev1"}]}
     mock_path = MagicMock(spec=Path)
+    mock_path.open = mock_open(read_data="dummy_stream")
     original_file_lines = ["repos:\n", "  - repo: repo1\n", "    rev: rev1\n"]
 
     config = PreCommitHookConfig(data, mock_path, original_file_lines=original_file_lines)
     config.original_file_lines = original_file_lines  # setup original file lines
     new_versions = {PreCommitRepo("repo1", "rev1"): "rev2"}
 
     mock_re.sub.return_value = "    rev: rev2\n"
     mock_diff.ndiff.return_value = ["- rev: rev1", "+ rev: rev2"]
 
     config.update_pre_commit_repo_versions(new_versions)
 
-    mock_open_file.assert_called_once_with(mock_path, "w")  # asserts the file is opened for writing
+    mock_path.open.assert_called_once_with("w")  # asserts the file is opened for writing
     mock_re.sub.assert_called_once_with(r"(?<=rev: )\S*", "rev2", "    rev: rev1\n")
     assert mock_diff.ndiff.called
 
 
 @patch("sync_pre_commit_lock.actions.sync_hooks.difflib")
 @patch("sync_pre_commit_lock.actions.sync_hooks.re")
 @patch("builtins.open", new_callable=mock_open)
```

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_actions/test_sync_hooks.py` & `sync_pre_commit_lock-0.1.1/tests/test_actions/test_sync_hooks.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_config.py` & `sync_pre_commit_lock-0.1.1/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,27 +38,29 @@
     assert config.dependency_mapping == {"pytest": {"repo": "pytest", "rev": "${ver}"}}
 
 
 @patch("sync_pre_commit_lock.config.toml.load", return_value={"tool": {"sync-pre-commit-lock": {}}})
 @patch("builtins.open", new_callable=MagicMock)
 def test_load_config_with_empty_tool_dict(mock_open: MagicMock, mock_load: MagicMock) -> None:
     expected_config = SyncPreCommitLockConfig()
-
-    actual_config = load_config()
+    mock_path = MagicMock()
+    mock_path.open = mock_open(read_data="dummy_stream")
+    actual_config = load_config(mock_path)
 
     assert actual_config == expected_config
-    mock_open.assert_called_once_with("pyproject.toml", "rb")
+    mock_path.open.assert_called_once_with("rb")
     mock_load.assert_called_once()
 
 
 @patch("sync_pre_commit_lock.config.toml.load", return_value={"tool": {"sync-pre-commit-lock": {"disable": True}}})
 @patch("builtins.open", new_callable=MagicMock)
 @patch("sync_pre_commit_lock.config.from_toml", return_value=SyncPreCommitLockConfig(disable_sync_from_lock=True))
 def test_load_config_with_data(mock_from_toml: MagicMock, mock_open: MagicMock, mock_load: MagicMock) -> None:
     expected_config = SyncPreCommitLockConfig(disable_sync_from_lock=True)
-
-    actual_config = load_config()
+    mock_path = MagicMock()
+    mock_path.open = mock_open(read_data="dummy_stream")
+    actual_config = load_config(mock_path)
 
     assert actual_config == expected_config
-    mock_open.assert_called_once_with("pyproject.toml", "rb")
+    mock_path.open.assert_called_once_with("rb")
     mock_load.assert_called_once()
     mock_from_toml.assert_called_once_with({"disable": True})
```

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_pdm/test_pdm_plugin.py` & `sync_pre_commit_lock-0.1.1/tests/test_pdm/test_pdm_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     ):
         from sync_pre_commit_lock.pdm_plugin import on_pdm_install_setup_pre_commit
 
         on_pdm_install_setup_pre_commit(project_mock, hooks=hooks_mock, candidates=candidates_mock, dry_run=False)
     printer_mock.debug.assert_any_call("Automatically installing pre-commit hooks is disabled. Skipping.")
 
 
-def test_on_pdm_install_setup_pre_commit_no_config_file() -> None:
+def test_on_pdm_install_setup_pre_commit_no_config_file(tmp_path: Path) -> None:
     config_mock.automatically_install_hooks = True
     config_mock.pre_commit_config_file = SyncPreCommitLockConfig.pre_commit_config_file
-    project_mock.root = Path("/tmp")
+    project_mock.root = tmp_path
     with mock.patch("sync_pre_commit_lock.pdm_plugin.PDMPrinter", return_value=printer_mock), mock.patch(
         "sync_pre_commit_lock.pdm_plugin.load_config", return_value=config_mock
     ):
         from sync_pre_commit_lock.pdm_plugin import on_pdm_install_setup_pre_commit
 
         on_pdm_install_setup_pre_commit(project_mock, hooks=hooks_mock, candidates=candidates_mock, dry_run=False)
     printer_mock.info.assert_called_once_with("No pre-commit config file found, skipping pre-commit hook check")
```

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_pdm/test_pdm_sync_pre_commit_hook.py` & `sync_pre_commit_lock-0.1.1/tests/test_pdm/test_pdm_sync_pre_commit_hook.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_poetry/test_poetry_plugin.py` & `sync_pre_commit_lock-0.1.1/tests/test_poetry/test_poetry_plugin.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/tests/test_utils.py` & `sync_pre_commit_lock-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sync_pre_commit_lock-0.1.0/PKG-INFO` & `sync_pre_commit_lock-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sync-pre-commit-lock
-Version: 0.1.0
+Version: 0.1.1
 Summary: PDM plugin to sync your pre-commit versions with your lockfile.
 Author-Email: Gabriel Dugny <sync-pre-commit-lock@dugny.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,18 +699,19 @@
 Requires-Dist: pdm>=2.7.4; extra == "pdm"
 Provides-Extra: pdm
 Description-Content-Type: text/markdown
 
 # sync-pre-commit-lock
 
 [![Tests](https://github.com/GabDug/sync-pre-commit-lock/actions/workflows/ci.yml/badge.svg)](https://github.com/GabDug/sync-pre-commit-lock/actions/workflows/ci.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/GabDug/sync-pre-commit-lock/main.svg)](https://results.pre-commit.ci/latest/github/GabDug/sync-pre-commit-lock/main)
+[![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7529/badge)](https://bestpractices.coreinfrastructure.org/projects/7529)
 [![pypi version](https://img.shields.io/pypi/v/sync-pre-commit-lock.svg)](https://pypi.org/project/sync-pre-commit-lock/)
 [![License](https://img.shields.io/pypi/l/sync-pre-commit-lock.svg)](https://pypi.python.org/pypi/sync-pre-commit-lock)
 [![Python version](https://img.shields.io/pypi/pyversions/sync-pre-commit-lock.svg)](https://pypi.python.org/pypi/sync-pre-commit-lock)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/GabDug/sync-pre-commit-lock/main.svg)](https://results.pre-commit.ci/latest/github/GabDug/sync-pre-commit-lock/main)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 [![Ruff](https://img.shields.io/badge/ruff-lint-red)](https://github.com/charliermarsh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 PDM and Poetry plugin to sync your pre-commit versions with your lockfile and automatically install pre-commit hooks.
 
 ## Features
@@ -746,37 +747,69 @@
 
 > We add the extra group `[pdm]` to the plugin name, to make sure version constraints are met.
 
 ### For Poetry
 
 Install like any other Poetry plugin, but beware that it's still in development!
 
-## TODO
+## Configuration
+
+This plugin is configured using the `tool.sync-pre-commit-lock` section in your `pyproject.toml` file.
+
+Here is the default configuration:
+
+```toml
+[tool.sync-pre-commit-lock]
+# Run `pre-commit install` automatically if applicable
+automaticall-install-hooks = true
+# Should we sync your pre-commit versions with your lockfile (when running lock, add, update, remove, etc.)?
+disable-sync-from_lock = false
+# Packages to ignore when syncing from lock
+ignore = []
+# Name of the pre-commit config file to sync with
+pre-commit-config-file = "pre-commit-config.yaml"
+# Additional mapping of URLs to python packages
+# Default is empty, but will merge with the default mapping
+# "rev" indicates the format of the Git tags
+dependency-mapping = {"package-name"= {"repo"= "https://github.com/example/package-name", "rev"= "v${rev}"}}
+```
+
+> Note: the `dependency-mapping` is merged with the default mapping, so you don't need to specify the default mapping if you want to add a new mapping.
+> Repos urls will be normalized to http(s), with the trailing slash removed.
 
-- [X] Add tests
-- [X] Add "E2E" tests
-- [X] Add CI (mypy, testing)
+## Usage
+
+Once installed, and optionally configured, the plugin usage should be transparent, and trigger when you run applicable PDM or Poetry commands.
+
+There should be a message in the output, when the sync or install or pre-commit is triggered.
+
+## Improvement ideas
+
+Feel free to open an issue or a PR if you have any idea, or if you want to help!
+
+### Release / CI / Dev
+
+- [ ] Upload build artifacts on GitHub release
+- [ ] Add a changelog
+- [ ] Add "E2E" tests
 - [ ] Add PDM scripts for dev and CI
-- [ ] Add CD (automated releases)
 - [ ] Add docs
-- [X] Add badges
-- [X] Add pre-commit hook to run linting
+
+### Features or fixes
+
 - [ ] Create a more verbose command
-- [X] Add support for poetry
-- [ ] Add support for hatch
-- [ ] Add support for flit
-- [ ] Add CLI?
+- [ ] Add support for other lockfiles / project managers (pipenv, flit, hatch, etc.)
+- [ ] Add a dedicated CLI command to manage sync/install
 - [ ] Expose a pre-commit hook to sync the lockfile
 - [ ] Support nested params for some repos? Like mypy types
-- [ ] Support reading DB from python module?
-- [ ] Support reordering DB inputs (file/global config/python module/cli)
-- [ ] Test using SSH/file dependencies
+- [ ] Support reading DB from a Python module?
+- [ ] Support reordering DB inputs (file/global config/python module/cli)?
+- [ ] Test using SSH/file dependencies?
 - [ ] Check ref existence before writing?
 - [ ] Support multiple hooks repos for the same dependency?
-- [X] Normalize the URL trailing slash
 - [ ] New feature to convert from pre-commit online to local?
 
 ## Inspiration
 
 This project is inspired by @floatingpurr's [sync_with_pdm](https://github.com/floatingpurr/sync_with_pdm/) and [sync_with_poetry](https://github.com/floatingpurr/sync_with_poetry/).
 
 The code to install pre-commit hooks automatically is **adapted** from @vstrimaitis's [poetry-pre-commit-plugin](https://github.com/vstrimaitis/poetry-pre-commit-plugin/), licensed under GPL-3.
```

