# Comparing `tmp/autonomy_dev-0.2.0.tar.gz` & `tmp/autonomy_dev-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.2.0.tar", max compression
+gzip compressed data, was "autonomy_dev-0.2.2.tar", max compression
```

## Comparing `autonomy_dev-0.2.0.tar` & `autonomy_dev-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,41 @@
--rw-r--r--   0        0        0      578 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/LICENSE
--rw-r--r--   0        0        0      368 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/__init__.py
--rw-r--r--   0        0        0     2569 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/base.py
--rw-r--r--   0        0        0      242 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/cli.py
--rw-r--r--   0        0        0     2758 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/cli_executor.py
--rw-r--r--   0        0        0     3335 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/augment.py
--rw-r--r--   0        0        0     1890 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/fmt.py
--rw-r--r--   0        0        0     2144 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/lint.py
--rw-r--r--   0        0        0     5195 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/repo.py
--rw-r--r--   0        0        0    10945 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/scaffold.py
--rw-r--r--   0        0        0     1450 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/test.py
--rw-r--r--   0        0        0      515 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/constants.py
--rw-r--r--   0        0        0      173 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/data/mermaid.py
--rw-r--r--   0        0        0      642 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      532 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/data/repo/templates/python/readme.py
--rw-r--r--   0        0        0     2027 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/fmt.py
--rw-r--r--   0        0        0      464 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/lint.py
--rw-r--r--   0        0        0     2153 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/local_fork.py
--rw-r--r--   0        0        0      470 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/test.py
--rw-r--r--   0        0        0     1585 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/utils.py
--rw-r--r--   0        0        0     2613 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      455 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1634 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_augmenter.py
--rw-r--r--   0        0        0     1108 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_cli.py
--rw-r--r--   0        0        0     2488 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_contracts.py
--rw-r--r--   0        0        0     1562 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_local_fork.py
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 autonomy_dev-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/LICENSE
+-rw-r--r--   0        0        0      913 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2569 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     3456 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     1890 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0      962 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/fsm.py
+-rw-r--r--   0        0        0     2144 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0     5195 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/repo.py
+-rw-r--r--   0        0        0     3400 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/scaffold.py
+-rw-r--r--   0        0        0     1450 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      515 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/constants.py
+-rw-r--r--   0        0        0     1482 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/block_explorer.py
+-rw-r--r--   0        0        0     5617 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract.py
+-rw-r--r--   0        0        0     2914 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract_functions.py
+-rw-r--r--   0        0        0     2238 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract_scafolder.py
+-rw-r--r--   0        0        0     6086 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/contract_templates.py
+-rw-r--r--   0        0        0     1493 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/function.py
+-rw-r--r--   0        0        0      525 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/param_type.py
+-rw-r--r--   0        0        0     1392 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/utils.py
+-rw-r--r--   0        0        0     1534 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/contracts/variable.py
+-rw-r--r--   0        0        0     1158 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/contracts/header.py
+-rw-r--r--   0        0        0      173 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      642 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      532 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/data/repo/templates/python/readme.py
+-rw-r--r--   0        0        0     2027 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/fmt.py
+-rw-r--r--   0        0        0     4084 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/fsm/fsm.py
+-rw-r--r--   0        0        0      464 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/lint.py
+-rw-r--r--   0        0        0     2153 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/local_fork.py
+-rw-r--r--   0        0        0      470 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/test.py
+-rw-r--r--   0        0        0     2542 2023-07-03 09:54:55.128104 autonomy_dev-0.2.2/auto_dev/utils.py
+-rw-r--r--   0        0        0     2635 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      296 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     1634 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1084 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_cli.py
+-rw-r--r--   0        0        0     2459 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_contracts.py
+-rw-r--r--   0        0        0     3626 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_fsm.py
+-rw-r--r--   0        0        0     1562 2023-07-03 09:54:55.132104 autonomy_dev-0.2.2/tests/test_local_fork.py
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 autonomy_dev-0.2.2/PKG-INFO
```

### Comparing `autonomy_dev-0.2.0/LICENSE` & `autonomy_dev-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/base.py` & `autonomy_dev-0.2.2/auto_dev/base.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/cli_executor.py` & `autonomy_dev-0.2.2/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/commands/augment.py` & `autonomy_dev-0.2.2/auto_dev/commands/augment.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     "logfile": LOGFILE_HANDLER,
 }
 
 
 def write(path: str, content: dict):
     """Safe write the contents to the path using yaml."""
     with open(path, "w", encoding=DEFAULT_ENCODING) as file:
-        yaml.dump(content, file, default_flow_style=False)
+        yaml.dump(content, file, default_flow_style=False, sort_keys=False)
 
 
 class LoggingScaffolder:
     """Logging scaffolder."""
 
     def __init__(self):
         """Init scaffolder."""
@@ -98,15 +98,20 @@
         return logging_config
 
     def scaffold(self, handlers: list):
         """Scaffold logging."""
         path = "aea-config.yaml"
         if not Path(path).exists():
             raise FileNotFoundError(f"File {path} not found")
-        aea_config = list(yaml.safe_load_all(Path(path).read_text(encoding=DEFAULT_ENCODING))).pop(0)
+
+        config = yaml.safe_load(Path(path).read_text(encoding=DEFAULT_ENCODING))
+        if isinstance(config, dict):
+            aea_config = config
+        else:
+            aea_config = list(config)[0]
         logging_config = self.generate(handlers)
         aea_config.update(logging_config)
         write(path, aea_config)
         return logging_config
 
 
 @cli.group()
```

### Comparing `autonomy_dev-0.2.0/auto_dev/commands/fmt.py` & `autonomy_dev-0.2.2/auto_dev/commands/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/commands/lint.py` & `autonomy_dev-0.2.2/auto_dev/commands/lint.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/commands/repo.py` & `autonomy_dev-0.2.2/auto_dev/commands/repo.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/commands/test.py` & `autonomy_dev-0.2.2/auto_dev/commands/test.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/constants.py` & `autonomy_dev-0.2.2/auto_dev/constants.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/data/pylama.ini` & `autonomy_dev-0.2.2/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/data/repo/templates/python/readme.py` & `autonomy_dev-0.2.2/auto_dev/data/repo/templates/python/readme.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/fmt.py` & `autonomy_dev-0.2.2/auto_dev/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/auto_dev/local_fork.py` & `autonomy_dev-0.2.2/auto_dev/local_fork.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/pyproject.toml` & `autonomy_dev-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.2.0"
+version = "0.2.2"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -48,18 +48,19 @@
 install = "^1.3.5"
 mkdocstrings-python = "^0.10.0"
 isort = "~5"
 pylint = "~2"
 open-aea = "^1.35.0"
 open-aea-cli-ipfs = "^1.35.0"
 web3 = "~5"
-responses = "^0.23.1"
-docker = "^6.1.3"
+open-autonomy = "^0.10"
+docker = "~6.1"
 
 [tool.poetry.dev-dependencies]
+responses = "^0.23.1"
 
 
 [tool.poetry.extras]
 all = [
     "pytest",
     "black",
     "isort",
```

### Comparing `autonomy_dev-0.2.0/tests/test_augmenter.py` & `autonomy_dev-0.2.2/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.2.0/tests/test_cli.py` & `autonomy_dev-0.2.2/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 @pytest.fixture
 def runner():
     """Fixture for invoking command-line interfaces."""
     return CliRunner()
 
 
-def test_lint_fails(runner, isolated_filesystem):
+def test_lint_fails(runner, test_filesystem):
     """Test the lint command fails with no packages."""
-    assert os.getcwd() == isolated_filesystem
+    assert os.getcwd() == test_filesystem
     result = runner.invoke(cli, ["lint"])
     assert result.exit_code == 1, result.output
     assert result.exception is not None
     assert isinstance(result.exception, FileNotFoundError)
 
 
-def test_lints_self(runner, isolated_filesystem):
+def test_lints_self(runner, test_filesystem):
     """Test the lint command works with the current package."""
-    assert os.getcwd() == isolated_filesystem
+    assert os.getcwd() == test_filesystem
     result = runner.invoke(cli, ["lint", "-p", "."])
     assert result.exit_code == 0, result.output
 
 
-def test_formats_self(runner, isolated_filesystem):
+def test_formats_self(runner, test_filesystem):
     """Test the format command works with the current package."""
-    assert os.getcwd() == isolated_filesystem
+    assert os.getcwd() == test_filesystem
     result = runner.invoke(cli, ["fmt", "-p", "."])
     assert result.exit_code == 0, result.output
```

### Comparing `autonomy_dev-0.2.0/tests/test_contracts.py` & `autonomy_dev-0.2.2/tests/test_contracts.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,49 +34,49 @@
     block_explorer = BlockExplorer(BLOCK_EXPLORER_URL, BLOCK_EXPLORER_API_KEY)
     abi = block_explorer.get_abi(KNOWN_ADDRESS)
     assert abi
 
 
 # we now test the scaffolder
 @pytest.fixture
-def scaffolder():
+def scaffolder(block_explorer):
     """
     Scaffolder fixture.
     """
-    return ContractScaffolder()
+    return ContractScaffolder(block_explorer, "eightballer")
 
 
 @responses.activate
-def test_scaffolder_generate(scaffolder, block_explorer):
+def test_scaffolder_generate(scaffolder):
     """Test the scaffolder."""
     responses.add(
         responses.GET,
         f"{BLOCK_EXPLORER_URL}/api?module=contract&action=getabi&address={KNOWN_ADDRESS}",
         json={"status": "1", "message": "OK", "result": '{"abi": "some_abi"}'},
     )
-    new_contract = scaffolder.from_block_explorer(block_explorer, KNOWN_ADDRESS, "new_contract")
+    new_contract = scaffolder.from_block_explorer(KNOWN_ADDRESS, "new_contract")
     assert new_contract
     assert new_contract.abi
     assert new_contract.address == KNOWN_ADDRESS
     assert new_contract.name == "new_contract"
     assert new_contract.author == "eightballer"
 
 
 @responses.activate
-def test_scaffolder_generate_openaea_contract(scaffolder, block_explorer, isolated_filesystem):
+def test_scaffolder_generate_openaea_contract(scaffolder, test_filesystem):
     """
     Test the scaffolder.
     """
-    del isolated_filesystem
+    del test_filesystem
     responses.add(
         responses.GET,
         f"{BLOCK_EXPLORER_URL}/api?module=contract&action=getabi&address={KNOWN_ADDRESS}",
         json={"status": "1", "message": "OK", "result": '{"abi": "some_abi"}'},
     )
-    new_contract = scaffolder.from_block_explorer(block_explorer, KNOWN_ADDRESS, "new_contract")
+    new_contract = scaffolder.from_block_explorer(KNOWN_ADDRESS, "new_contract")
     contract_path = scaffolder.generate_openaea_contract(new_contract)
     assert contract_path
     assert contract_path.exists()
     assert contract_path.name == "new_contract"
     assert contract_path.parent.name == "contracts"
     shutil.rmtree(contract_path.parent)
     assert not contract_path.exists()
```

### Comparing `autonomy_dev-0.2.0/tests/test_local_fork.py` & `autonomy_dev-0.2.2/tests/test_local_fork.py`

 * *Files identical despite different names*

