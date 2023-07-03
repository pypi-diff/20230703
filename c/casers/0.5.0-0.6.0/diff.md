# Comparing `tmp/casers-0.5.0.tar.gz` & `tmp/casers-0.6.0.tar.gz`

## Comparing `casers-0.5.0.tar` & `casers-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 casers-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123      932 2023-05-13 15:14:45.000000 casers-0.5.0/.github/ISSUE_TEMPLATE/issue.yaml
--rw-r--r--   0     1001      123      182 2023-05-13 15:14:45.000000 casers-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0     1001      123      411 2023-05-13 15:14:45.000000 casers-0.5.0/.github/workflows/bumpversion.yml
--rw-r--r--   0     1001      123      586 2023-05-13 15:14:45.000000 casers-0.5.0/.github/workflows/check.yml
--rw-r--r--   0     1001      123     2767 2023-05-13 15:14:45.000000 casers-0.5.0/.github/workflows/maturin.yml
--rw-r--r--   0     1001      123      302 2023-05-13 15:14:45.000000 casers-0.5.0/.github/workflows/pr.yml
--rw-r--r--   0     1001      123     1813 2023-05-13 15:14:45.000000 casers-0.5.0/.gitignore
--rw-r--r--   0     1001      123      542 2023-05-13 15:14:45.000000 casers-0.5.0/CHANGELOG.md
--rw-r--r--   0     1001      123      135 2023-05-13 15:14:45.000000 casers-0.5.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123     2847 2023-05-13 15:14:45.000000 casers-0.5.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1092 2023-05-13 15:14:45.000000 casers-0.5.0/LICENSE
--rw-r--r--   0     1001      123     1758 2023-05-13 15:14:45.000000 casers-0.5.0/Makefile
--rw-r--r--   0     1001      123     1412 2023-05-13 15:14:45.000000 casers-0.5.0/README.md
--rw-r--r--   0     1001      123        0 2023-05-13 15:14:45.000000 casers-0.5.0/benches/__init__.py
--rw-r--r--   0     1001      123     1810 2023-05-13 15:14:45.000000 casers-0.5.0/benches/main.py
--rw-r--r--   0     1001      123      282 2023-05-13 15:14:45.000000 casers-0.5.0/casers/__init__.py
--rw-r--r--   0     1001      123       32 2023-05-13 15:14:45.000000 casers-0.5.0/casers/__main__.py
--rw-r--r--   0     1001      123       66 2023-05-13 15:14:45.000000 casers-0.5.0/casers/_casers.pyi
--rw-r--r--   0     1001      123      462 2023-05-13 15:14:45.000000 casers-0.5.0/casers/_extra.py
--rw-r--r--   0     1001      123       22 2023-05-13 15:14:45.000000 casers-0.5.0/casers/_version.py
--rw-r--r--   0     1001      123        0 2023-05-13 15:14:45.000000 casers-0.5.0/casers/cli/__init__.py
--rw-r--r--   0     1001      123      360 2023-05-13 15:14:45.000000 casers-0.5.0/casers/cli/app.py
--rw-r--r--   0     1001      123        1 2023-05-13 15:14:45.000000 casers-0.5.0/casers/py.typed
--rw-r--r--   0     1001      123      394 2023-05-13 15:14:45.000000 casers-0.5.0/casers/pydantic.py
--rw-r--r--   0     1001      123    64193 2023-05-13 15:14:45.000000 casers-0.5.0/poetry.lock
--rw-r--r--   0     1001      123     3032 2023-05-13 15:14:45.000000 casers-0.5.0/pyproject.toml
--rw-r--r--   0     1001      123     1860 2023-05-13 15:14:45.000000 casers-0.5.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-05-13 15:14:45.000000 casers-0.5.0/tests/__init__.py
--rw-r--r--   0     1001      123      340 2023-05-13 15:14:45.000000 casers-0.5.0/tests/test_pydantic.py
--rw-r--r--   0     1001      123      343 2023-05-13 15:14:45.000000 casers-0.5.0/tests/test_to_camel.py
--rw-r--r--   0     1001      123      554 2023-05-13 15:14:45.000000 casers-0.5.0/tests/test_to_constant.py
--rw-r--r--   0     1001      123      545 2023-05-13 15:14:45.000000 casers-0.5.0/tests/test_to_kebab.py
--rw-r--r--   0     1001      123      346 2023-05-13 15:14:45.000000 casers-0.5.0/tests/test_to_pascal.py
--rw-r--r--   0     1001      123      618 2023-05-13 15:14:45.000000 casers-0.5.0/tests/test_to_snake.py
--rw-r--r--   0     1001      123     7650 2023-05-13 15:15:59.000000 casers-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 casers-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      237 1970-01-01 00:00:00.000000 casers-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      123      932 2023-07-03 15:49:02.000000 casers-0.6.0/.github/ISSUE_TEMPLATE/issue.yaml
+-rw-r--r--   0     1001      123      182 2023-07-03 15:49:02.000000 casers-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0     1001      123      411 2023-07-03 15:49:02.000000 casers-0.6.0/.github/workflows/bumpversion.yml
+-rw-r--r--   0     1001      123      586 2023-07-03 15:49:02.000000 casers-0.6.0/.github/workflows/check.yml
+-rw-r--r--   0     1001      123     2767 2023-07-03 15:49:02.000000 casers-0.6.0/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      123      302 2023-07-03 15:49:02.000000 casers-0.6.0/.github/workflows/pr.yml
+-rw-r--r--   0     1001      123     1813 2023-07-03 15:49:02.000000 casers-0.6.0/.gitignore
+-rw-r--r--   0     1001      123      605 2023-07-03 15:49:02.000000 casers-0.6.0/CHANGELOG.md
+-rw-r--r--   0     1001      123      135 2023-07-03 15:49:02.000000 casers-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123     2847 2023-07-03 15:49:02.000000 casers-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1092 2023-07-03 15:49:02.000000 casers-0.6.0/LICENSE
+-rw-r--r--   0     1001      123     1758 2023-07-03 15:49:02.000000 casers-0.6.0/Makefile
+-rw-r--r--   0     1001      123     1493 2023-07-03 15:49:02.000000 casers-0.6.0/README.md
+-rw-r--r--   0     1001      123        0 2023-07-03 15:49:02.000000 casers-0.6.0/benches/__init__.py
+-rw-r--r--   0     1001      123     1810 2023-07-03 15:49:02.000000 casers-0.6.0/benches/main.py
+-rw-r--r--   0     1001      123      282 2023-07-03 15:49:02.000000 casers-0.6.0/casers/__init__.py
+-rw-r--r--   0     1001      123       32 2023-07-03 15:49:02.000000 casers-0.6.0/casers/__main__.py
+-rw-r--r--   0     1001      123       66 2023-07-03 15:49:02.000000 casers-0.6.0/casers/_casers.pyi
+-rw-r--r--   0     1001      123      462 2023-07-03 15:49:02.000000 casers-0.6.0/casers/_extra.py
+-rw-r--r--   0     1001      123       22 2023-07-03 15:49:02.000000 casers-0.6.0/casers/_version.py
+-rw-r--r--   0     1001      123        0 2023-07-03 15:49:02.000000 casers-0.6.0/casers/cli/__init__.py
+-rw-r--r--   0     1001      123      360 2023-07-03 15:49:02.000000 casers-0.6.0/casers/cli/app.py
+-rw-r--r--   0     1001      123        1 2023-07-03 15:49:02.000000 casers-0.6.0/casers/py.typed
+-rw-r--r--   0     1001      123      910 2023-07-03 15:49:02.000000 casers-0.6.0/casers/pydantic.py
+-rw-r--r--   0     1001      123    72396 2023-07-03 15:49:02.000000 casers-0.6.0/poetry.lock
+-rw-r--r--   0     1001      123     3108 2023-07-03 15:49:02.000000 casers-0.6.0/pyproject.toml
+-rw-r--r--   0     1001      123     1860 2023-07-03 15:49:02.000000 casers-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-07-03 15:49:02.000000 casers-0.6.0/tests/__init__.py
+-rw-r--r--   0     1001      123     1013 2023-07-03 15:49:02.000000 casers-0.6.0/tests/test_pydantic.py
+-rw-r--r--   0     1001      123      343 2023-07-03 15:49:02.000000 casers-0.6.0/tests/test_to_camel.py
+-rw-r--r--   0     1001      123      554 2023-07-03 15:49:02.000000 casers-0.6.0/tests/test_to_constant.py
+-rw-r--r--   0     1001      123      545 2023-07-03 15:49:02.000000 casers-0.6.0/tests/test_to_kebab.py
+-rw-r--r--   0     1001      123      346 2023-07-03 15:49:02.000000 casers-0.6.0/tests/test_to_pascal.py
+-rw-r--r--   0     1001      123      618 2023-07-03 15:49:02.000000 casers-0.6.0/tests/test_to_snake.py
+-rw-r--r--   0     1001      123     7650 2023-07-03 15:49:10.000000 casers-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 casers-0.6.0/PKG-INFO
```

### Comparing `casers-0.5.0/.github/ISSUE_TEMPLATE/issue.yaml` & `casers-0.6.0/.github/ISSUE_TEMPLATE/issue.yaml`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/.github/workflows/check.yml` & `casers-0.6.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/.github/workflows/maturin.yml` & `casers-0.6.0/.github/workflows/maturin.yml`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/.gitignore` & `casers-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/CHANGELOG.md` & `casers-0.6.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.6.0 (2023-07-03)
+
+### Feat
+
+- supporting for pydantic v2
+
 ## 0.5.0 (2023-05-13)
 
 ### Feat
 
 - add to_constant, to_kebab, to_pascal
 
 ## 0.4.0 (2023-04-18)
```

### Comparing `casers-0.5.0/CONTRIBUTING.md` & `casers-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/LICENSE` & `casers-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/Makefile` & `casers-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/README.md` & `casers-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,27 @@
 >>> to_kebab("someText") == "some-text"
 True
 >>> to_kebab("some_text") == "some-text"
 True
 
 ```
 
+### pydantic
+
+The package supports for pydantic 1 and 2 versions
+
 ```python
 >>> from casers.pydantic import CamelAliases
 
 >>> class Model(CamelAliases):
 ...     snake_case: str
 
->>> Model.parse_obj({"snakeCase": "value"}).snake_case == "value"
+>>> Model.model_validate({"snakeCase": "value"}).snake_case == "value"
 True
->>> Model.parse_raw('{"snakeCase": "value"}').snake_case == "value"
+>>> Model.model_validate_json('{"snakeCase": "value"}').snake_case == "value"
 True
 
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
```

### Comparing `casers-0.5.0/benches/main.py` & `casers-0.6.0/benches/main.py`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/poetry.lock` & `casers-0.6.0/poetry.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,27 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
+
+[[package]]
+name = "annotated-types"
+version = "0.5.0"
+description = "Reusable constraint types to use with typing.Annotated"
+optional = true
+python-versions = ">=3.7"
+files = [
+    {file = "annotated_types-0.5.0-py3-none-any.whl", hash = "sha256:58da39888f92c276ad970249761ebea80ba544b77acddaa1a4d6cf78287d45fd"},
+    {file = "annotated_types-0.5.0.tar.gz", hash = "sha256:47cdc3490d9ac1506ce92c7aaa76c579dc3509ff11e098fc867e5130ab7be802"},
+]
+
+[package.dependencies]
+typing-extensions = {version = ">=4.0.0", markers = "python_version < \"3.9\""}
 
 [[package]]
 name = "argcomplete"
 version = "2.0.6"
 description = "Bash tab completion for argparse"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "argcomplete-2.0.6-py3-none-any.whl", hash = "sha256:6c2170b3e0ab54683cb28d319b65261bde1f11388be688b68118b7d281e34c94"},
     {file = "argcomplete-2.0.6.tar.gz", hash = "sha256:dc33528d96727882b576b24bc89ed038f3c6abbb6855ff9bb6be23384afff9d6"},
 ]
 
@@ -19,15 +32,14 @@
 lint = ["flake8", "mypy"]
 test = ["coverage", "flake8", "mypy", "pexpect", "wheel"]
 
 [[package]]
 name = "black"
 version = "23.3.0"
 description = "The uncompromising code formatter."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
     {file = "black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
@@ -70,30 +82,28 @@
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "charset-normalizer"
 version = "2.1.1"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
-category = "dev"
 optional = false
 python-versions = ">=3.6.0"
 files = [
     {file = "charset-normalizer-2.1.1.tar.gz", hash = "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845"},
     {file = "charset_normalizer-2.1.1-py3-none-any.whl", hash = "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"},
 ]
 
 [package.extras]
 unicode-backport = ["unicodedata2"]
 
 [[package]]
 name = "click"
 version = "8.1.3"
 description = "Composable command line interface toolkit"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
     {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
 ]
 
@@ -101,27 +111,25 @@
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
-category = "dev"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "commitizen"
 version = "2.42.1"
 description = "Python commitizen client tool"
-category = "dev"
 optional = false
 python-versions = ">=3.6.2,<4.0.0"
 files = [
     {file = "commitizen-2.42.1-py3-none-any.whl", hash = "sha256:fad7d37cfae361a859b713d4ac591859d5ca03137dd52de4e1bd208f7f45d5dc"},
     {file = "commitizen-2.42.1.tar.gz", hash = "sha256:eac18c7c65587061aac6829534907aeb208405b8230bfd35ec08503c228a7f17"},
 ]
 
@@ -138,15 +146,14 @@
 tomlkit = ">=0.5.3,<1.0.0"
 typing-extensions = ">=4.0.1,<5.0.0"
 
 [[package]]
 name = "coverage"
 version = "7.2.3"
 description = "Code coverage measurement for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "coverage-7.2.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5"},
     {file = "coverage-7.2.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4"},
     {file = "coverage-7.2.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2"},
     {file = "coverage-7.2.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013"},
@@ -205,42 +212,39 @@
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "decli"
 version = "0.5.2"
 description = "Minimal, easy-to-use, declarative cli tool"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "decli-0.5.2-py3-none-any.whl", hash = "sha256:d3207bc02d0169bf6ed74ccca09ce62edca0eb25b0ebf8bf4ae3fb8333e15ca0"},
     {file = "decli-0.5.2.tar.gz", hash = "sha256:f2cde55034a75c819c630c7655a844c612f2598c42c21299160465df6ad463ad"},
 ]
 
 [[package]]
 name = "exceptiongroup"
 version = "1.1.1"
 description = "Backport of PEP 654 (exception groups)"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
     {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "importlib-metadata"
 version = "5.2.0"
 description = "Read metadata from Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "importlib_metadata-5.2.0-py3-none-any.whl", hash = "sha256:0eafa39ba42bf225fc00e67f701d71f85aead9f878569caf13c3724f704b970f"},
     {file = "importlib_metadata-5.2.0.tar.gz", hash = "sha256:404d48d62bba0b7a77ff9d405efd91501bef2e67ff4ace0bed40a0cf28c3c7cd"},
 ]
 
@@ -253,27 +257,25 @@
 perf = ["ipython"]
 testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
 
 [[package]]
 name = "iniconfig"
 version = "2.0.0"
 description = "brain-dead simple config-ini parsing"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "iniconfig-2.0.0-py3-none-any.whl", hash = "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"},
     {file = "iniconfig-2.0.0.tar.gz", hash = "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3"},
 ]
 
 [[package]]
 name = "jinja2"
 version = "3.1.2"
 description = "A very fast and expressive template engine."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
     {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
 ]
 
@@ -283,15 +285,14 @@
 [package.extras]
 i18n = ["Babel (>=2.7)"]
 
 [[package]]
 name = "markupsafe"
 version = "2.1.2"
 description = "Safely add untrusted strings to HTML/XML markup."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7"},
     {file = "MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036"},
     {file = "MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1"},
     {file = "MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323"},
@@ -343,15 +344,14 @@
     {file = "MarkupSafe-2.1.2.tar.gz", hash = "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d"},
 ]
 
 [[package]]
 name = "maturin"
 version = "0.14.17"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
-category = "dev"
 optional = false
 python-versions = ">= 3.7"
 files = [
     {file = "maturin-0.14.17-py3-none-linux_armv6l.whl", hash = "sha256:2684302ded1559a26635ec45e91ae7913aeb386a8b658d5c2eb13ff410df7930"},
     {file = "maturin-0.14.17-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:7fef3950a34c0b5c1806637169fca12f89b7440d7608832bf7765b34f394b06a"},
     {file = "maturin-0.14.17-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:a7f06984bd3ffa4ab7be67f7352353a486f262d7a0dbd4dc305944e0b09c8f35"},
     {file = "maturin-0.14.17-py3-none-manylinux_2_12_i686.manylinux2010_i686.musllinux_1_1_i686.whl", hash = "sha256:cf1429a7854ecd4830bb42407d30ff0625c3f6480fa7b1e90da2896ba7a1b2fc"},
@@ -373,15 +373,14 @@
 patchelf = ["patchelf"]
 zig = ["ziglang (>=0.10.0,<0.11.0)"]
 
 [[package]]
 name = "mypy"
 version = "1.2.0"
 description = "Optional static typing for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "mypy-1.2.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d"},
     {file = "mypy-1.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"},
     {file = "mypy-1.2.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e"},
     {file = "mypy-1.2.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a"},
@@ -421,51 +420,47 @@
 python2 = ["typed-ast (>=1.4.0,<2)"]
 reports = ["lxml"]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 description = "Type system extensions for programs checked with the mypy type checker."
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "packaging"
-version = "23.0"
+version = "23.1"
 description = "Core utilities for Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
-    {file = "packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
+    {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
+    {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "pathspec"
 version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
     {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
 version = "3.2.0"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "platformdirs-3.2.0-py3-none-any.whl", hash = "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"},
     {file = "platformdirs-3.2.0.tar.gz", hash = "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08"},
 ]
 
@@ -476,15 +471,14 @@
 docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.2.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pluggy"
 version = "1.0.0"
 description = "plugin and hook calling mechanisms for python"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "pluggy-1.0.0-py2.py3-none-any.whl", hash = "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"},
     {file = "pluggy-1.0.0.tar.gz", hash = "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159"},
 ]
 
@@ -495,83 +489,143 @@
 dev = ["pre-commit", "tox"]
 testing = ["pytest", "pytest-benchmark"]
 
 [[package]]
 name = "prompt-toolkit"
 version = "3.0.38"
 description = "Library for building powerful interactive command lines in Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7.0"
 files = [
     {file = "prompt_toolkit-3.0.38-py3-none-any.whl", hash = "sha256:45ea77a2f7c60418850331366c81cf6b5b9cf4c7fd34616f733c5427e6abbb1f"},
     {file = "prompt_toolkit-3.0.38.tar.gz", hash = "sha256:23ac5d50538a9a38c8bde05fecb47d0b403ecd0662857a86f886f798563d5b9b"},
 ]
 
 [package.dependencies]
 wcwidth = "*"
 
 [[package]]
 name = "pydantic"
-version = "1.10.7"
-description = "Data validation and settings management using python type hints"
-category = "main"
+version = "2.0"
+description = "Data validation using Python type hints"
 optional = true
 python-versions = ">=3.7"
 files = [
-    {file = "pydantic-1.10.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e79e999e539872e903767c417c897e729e015872040e56b96e67968c3b918b2d"},
-    {file = "pydantic-1.10.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:01aea3a42c13f2602b7ecbbea484a98169fb568ebd9e247593ea05f01b884b2e"},
-    {file = "pydantic-1.10.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:516f1ed9bc2406a0467dd777afc636c7091d71f214d5e413d64fef45174cfc7a"},
-    {file = "pydantic-1.10.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ae150a63564929c675d7f2303008d88426a0add46efd76c3fc797cd71cb1b46f"},
-    {file = "pydantic-1.10.7-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:ecbbc51391248116c0a055899e6c3e7ffbb11fb5e2a4cd6f2d0b93272118a209"},
-    {file = "pydantic-1.10.7-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:f4a2b50e2b03d5776e7f21af73e2070e1b5c0d0df255a827e7c632962f8315af"},
-    {file = "pydantic-1.10.7-cp310-cp310-win_amd64.whl", hash = "sha256:a7cd2251439988b413cb0a985c4ed82b6c6aac382dbaff53ae03c4b23a70e80a"},
-    {file = "pydantic-1.10.7-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:68792151e174a4aa9e9fc1b4e653e65a354a2fa0fed169f7b3d09902ad2cb6f1"},
-    {file = "pydantic-1.10.7-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:dfe2507b8ef209da71b6fb5f4e597b50c5a34b78d7e857c4f8f3115effaef5fe"},
-    {file = "pydantic-1.10.7-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:10a86d8c8db68086f1e30a530f7d5f83eb0685e632e411dbbcf2d5c0150e8dcd"},
-    {file = "pydantic-1.10.7-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d75ae19d2a3dbb146b6f324031c24f8a3f52ff5d6a9f22f0683694b3afcb16fb"},
-    {file = "pydantic-1.10.7-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:464855a7ff7f2cc2cf537ecc421291b9132aa9c79aef44e917ad711b4a93163b"},
-    {file = "pydantic-1.10.7-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:193924c563fae6ddcb71d3f06fa153866423ac1b793a47936656e806b64e24ca"},
-    {file = "pydantic-1.10.7-cp311-cp311-win_amd64.whl", hash = "sha256:b4a849d10f211389502059c33332e91327bc154acc1845f375a99eca3afa802d"},
-    {file = "pydantic-1.10.7-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:cc1dde4e50a5fc1336ee0581c1612215bc64ed6d28d2c7c6f25d2fe3e7c3e918"},
-    {file = "pydantic-1.10.7-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e0cfe895a504c060e5d36b287ee696e2fdad02d89e0d895f83037245218a87fe"},
-    {file = "pydantic-1.10.7-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:670bb4683ad1e48b0ecb06f0cfe2178dcf74ff27921cdf1606e527d2617a81ee"},
-    {file = "pydantic-1.10.7-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:950ce33857841f9a337ce07ddf46bc84e1c4946d2a3bba18f8280297157a3fd1"},
-    {file = "pydantic-1.10.7-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:c15582f9055fbc1bfe50266a19771bbbef33dd28c45e78afbe1996fd70966c2a"},
-    {file = "pydantic-1.10.7-cp37-cp37m-win_amd64.whl", hash = "sha256:82dffb306dd20bd5268fd6379bc4bfe75242a9c2b79fec58e1041fbbdb1f7914"},
-    {file = "pydantic-1.10.7-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:8c7f51861d73e8b9ddcb9916ae7ac39fb52761d9ea0df41128e81e2ba42886cd"},
-    {file = "pydantic-1.10.7-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:6434b49c0b03a51021ade5c4daa7d70c98f7a79e95b551201fff682fc1661245"},
-    {file = "pydantic-1.10.7-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:64d34ab766fa056df49013bb6e79921a0265204c071984e75a09cbceacbbdd5d"},
-    {file = "pydantic-1.10.7-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:701daea9ffe9d26f97b52f1d157e0d4121644f0fcf80b443248434958fd03dc3"},
-    {file = "pydantic-1.10.7-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:cf135c46099ff3f919d2150a948ce94b9ce545598ef2c6c7bf55dca98a304b52"},
-    {file = "pydantic-1.10.7-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:b0f85904f73161817b80781cc150f8b906d521fa11e3cdabae19a581c3606209"},
-    {file = "pydantic-1.10.7-cp38-cp38-win_amd64.whl", hash = "sha256:9f6f0fd68d73257ad6685419478c5aece46432f4bdd8d32c7345f1986496171e"},
-    {file = "pydantic-1.10.7-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c230c0d8a322276d6e7b88c3f7ce885f9ed16e0910354510e0bae84d54991143"},
-    {file = "pydantic-1.10.7-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:976cae77ba6a49d80f461fd8bba183ff7ba79f44aa5cfa82f1346b5626542f8e"},
-    {file = "pydantic-1.10.7-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7d45fc99d64af9aaf7e308054a0067fdcd87ffe974f2442312372dfa66e1001d"},
-    {file = "pydantic-1.10.7-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d2a5ebb48958754d386195fe9e9c5106f11275867051bf017a8059410e9abf1f"},
-    {file = "pydantic-1.10.7-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:abfb7d4a7cd5cc4e1d1887c43503a7c5dd608eadf8bc615413fc498d3e4645cd"},
-    {file = "pydantic-1.10.7-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:80b1fab4deb08a8292d15e43a6edccdffa5377a36a4597bb545b93e79c5ff0a5"},
-    {file = "pydantic-1.10.7-cp39-cp39-win_amd64.whl", hash = "sha256:d71e69699498b020ea198468e2480a2f1e7433e32a3a99760058c6520e2bea7e"},
-    {file = "pydantic-1.10.7-py3-none-any.whl", hash = "sha256:0cd181f1d0b1d00e2b705f1bf1ac7799a2d938cce3376b8007df62b29be3c2c6"},
-    {file = "pydantic-1.10.7.tar.gz", hash = "sha256:cfc83c0678b6ba51b0532bea66860617c4cd4251ecf76e9846fa5a9f3454e97e"},
+    {file = "pydantic-2.0-py3-none-any.whl", hash = "sha256:8bf7355be5e1207c756dfbc8046236dadd4ce04101fb482e6c8834a06d9aa04f"},
+    {file = "pydantic-2.0.tar.gz", hash = "sha256:6e313661b310eb5b2c45168ce05d8dd79f57563adaf3906162a917585576b846"},
 ]
 
 [package.dependencies]
-typing-extensions = ">=4.2.0"
+annotated-types = ">=0.4.0"
+pydantic-core = "2.0.1"
+typing-extensions = ">=4.6.1"
 
 [package.extras]
-dotenv = ["python-dotenv (>=0.10.4)"]
-email = ["email-validator (>=1.0.3)"]
+email = ["email-validator (>=2.0.0)"]
+
+[[package]]
+name = "pydantic-core"
+version = "2.0.1"
+description = ""
+optional = true
+python-versions = ">=3.7"
+files = [
+    {file = "pydantic_core-2.0.1-cp310-cp310-macosx_10_7_x86_64.whl", hash = "sha256:92b01e166a3b69e8054308709acabec1bae65dae83ba6329f4fcc8448e170a06"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ae53240f9f92f634b73a3e5ee87b9ec8ac38d5bee96ea65034af58f48d489a65"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e0dd6bb98271519a309e96e927b52f8ca1323a99762bec87cda8fdaaa221e5cd"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c656b8d4603af6744ed2f2c0be499790f0913a2186ef7214c88d47d42051ae4b"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-manylinux_2_24_armv7l.whl", hash = "sha256:ddbad540cba15b5262bd800bb6f0746a4ac719de0fe0a2acab8e0d50eb54ba9a"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-manylinux_2_24_ppc64le.whl", hash = "sha256:e2e9025e132761e7ea8dab448923ccd8839c60199e863a6348d7e8b1a674edd1"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-manylinux_2_24_s390x.whl", hash = "sha256:ac6a57d01c0b67563dd273f2b71e9aab643573b569a202bfff7dad502b0b8ee0"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:44c8cec1d74d74c29da59c86e8cd472851c85b44d75128096ef3751c5c87c204"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:76d5d18ef9065ecbf62d6ec82c45ddbb47174a7400eb780040a7ebdad1c0ead8"},
+    {file = "pydantic_core-2.0.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:722aa193ba1f587226991a789a3f098235b5f04e85cf815af9e8ad823a5a85e1"},
+    {file = "pydantic_core-2.0.1-cp310-none-win32.whl", hash = "sha256:16977790d69bac6034baa2349326db2ff465ad346c53b8d54c3674e05b070af2"},
+    {file = "pydantic_core-2.0.1-cp310-none-win_amd64.whl", hash = "sha256:0fcdb43190588f6219709b43ffa679e562c0d4a44a50aafb6cc88978da4a84b7"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-macosx_10_7_x86_64.whl", hash = "sha256:73c464afa0a959472045f242ef7cdaf6a38b76a6d7dfa1ef270de0967c04408d"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:ab7eafb33fdc7aa8667634be58a3d1c8ed3fa8923c6bc5014657bf95b51b4a46"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6cf3e484bc8e8c8a568d572a6619696d7e2e2aef214b0be503f0814f8bafca9f"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bc99af5be239961d718bbf8e4d6bd1caa6de556e44ed08eb5135cfbefc958728"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-manylinux_2_24_armv7l.whl", hash = "sha256:e55fc76ce657208c0d7e21e2e96925993dd4063d5c5ee9227dcdf4e550c02a29"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-manylinux_2_24_ppc64le.whl", hash = "sha256:ccb06e1667a9784a96e0fc2500b989b8afbe9ac68a39a3c806c056ee228eff3c"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-manylinux_2_24_s390x.whl", hash = "sha256:b23ae8b27b6eff72909a9a88123ac28b746d95f25927ce67d3b0f3dabe099a0a"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:6387c2956baf16891e7bc20d864a769c0f9f61799d4895c8f493e2de8f7b88aa"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:1c855ef11370eacff25556658fb7fa243e8c0bd4235fa20a0f473bded2ede252"},
+    {file = "pydantic_core-2.0.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f9452d470012ee86a00a36f7673843038fd1a88661a28c72e65e7f3f084da8d8"},
+    {file = "pydantic_core-2.0.1-cp311-none-win32.whl", hash = "sha256:0872a1c52da4cfc494e23c83532c7fc1313de311a14334b7a58216a8dea828e0"},
+    {file = "pydantic_core-2.0.1-cp311-none-win_amd64.whl", hash = "sha256:7a4fc3e8c788798739f4aa6772d994e4453a17dadb1b8eea4582a31cdfe683d2"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-macosx_10_7_x86_64.whl", hash = "sha256:ddb23eaf427dbbde41b543d98a0c4a7aeb73bf649e3faa75b94a2fd882a669ba"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-macosx_11_0_arm64.whl", hash = "sha256:4eda2b350b02293c7060f2371ad3ce7b00342bd61c8654d2ba374bd10c6b6b66"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7727a4fcb93572d4e521b028f1c64f1eda2da49d506b1a6208576faa9e0acd64"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:007cdcee7e1a40951768d0d250e566b603e25d0fa8b8302901e38560bc9badf9"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-manylinux_2_24_armv7l.whl", hash = "sha256:89123ab11a23fa9c332655933350dc231945ca6b1148c1e1960aad0a5a6de1c0"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-manylinux_2_24_ppc64le.whl", hash = "sha256:03d12c44decb122d5feede5408cc6c67e506b64016ce4b59c825d1a8c90f288a"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-manylinux_2_24_s390x.whl", hash = "sha256:ff015389ae4ca6869a2fdd16c21ee1ce7c134503f2148efd46db643ce27ca520"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:8daded5c64811da4bdc7d6792afa10328bff5c3514536f69457596d4a2646b49"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:a1dd1b182fde9f95f1cc28964612fb1b180fdd3ca2cac881c108db29906b2e01"},
+    {file = "pydantic_core-2.0.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:c8e53bae6e58a8ff8e93f9a77440cfe8fc017bb9a8430dc03beb6bdd648572d2"},
+    {file = "pydantic_core-2.0.1-cp37-none-win32.whl", hash = "sha256:a7d0de538719feda5cabf19c63cc17345df6a0ab579b95518925d2b25276daaf"},
+    {file = "pydantic_core-2.0.1-cp37-none-win_amd64.whl", hash = "sha256:1bb6d1057c054056614aefeced05299d3590acf76768538b34ebec9cbbf26953"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-macosx_10_7_x86_64.whl", hash = "sha256:9ee1c2d0cf5c92faf722ff366814859c764c82b30af7f91b9b1950e15efecb9e"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:adc2efaf0c45135214dff4d18d4aaf2b692249cb369f921fe0fde3a13cf7ddad"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8927c166f20e3933cc9a9a68701acc8de22ee54b70d8c4044ad461b043b3cf9b"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:adbfc6c7ddd1cca6efe62a0292cae7cf2d05c9ebb139d0da10b0d44346e253c7"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-manylinux_2_24_armv7l.whl", hash = "sha256:659f22427d653769d1b4c672fd2daf53e639a5a93b0dd6fc0b37ef822a6e77d7"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-manylinux_2_24_ppc64le.whl", hash = "sha256:71cf43912edeae476f47d16520e48bddbf9af0ebdd98961c38ca8944f4f22b9d"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-manylinux_2_24_s390x.whl", hash = "sha256:10736490eacc426d681ae6f00f1d8ce01fc77c45086a597e829c3eed127179b1"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:5f3158cb4cda580f3b063b03257c7f5c2d9e66f9c2a93466c76056f7c4d5a3b7"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:8ca5a743af642700fc69dc64e0b964dd7499dcabb399e5cc2223fbc9cb33965d"},
+    {file = "pydantic_core-2.0.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fa5a3d49ddbeaa80bb2a8927b90e9cdd43373616ba0b7b7a74a3ae33b5c9640c"},
+    {file = "pydantic_core-2.0.1-cp38-none-win32.whl", hash = "sha256:d6e21da7f7e3935b24bfd17d7c3eefe4c1edca380edaec854a8593796d8d96f1"},
+    {file = "pydantic_core-2.0.1-cp38-none-win_amd64.whl", hash = "sha256:0b154abef540a76bb2b7a641b3ae1e05e5c4b08eb9ad6c27a217b3c64ffcda0b"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-macosx_10_7_x86_64.whl", hash = "sha256:aad8b177370002f73f08eafefa3d969d9c4498da6d67d8a43ffdeb4b4e560e1c"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9cf1ba93657cad863d23ecb09227665c0abe26c131acd24abb5edc6249a36a70"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:79225132aa1fe97a5e947da820b323d63372fb3475d94ff81ca6f91669717a01"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7bd78c4f04794a8e527d32c8ec1a26682b35b5c9347bb6e3cc853ba1a43c72a5"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-manylinux_2_24_armv7l.whl", hash = "sha256:bb2daa4e3d4efbf2e2dedc1a7cea3e48ff12d0c95ab2011e7f731bdc97d16ed0"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-manylinux_2_24_ppc64le.whl", hash = "sha256:958964a0ad0cea700b25037b21f5a2da38d19bddaa2f15ce36f51c048a9efe92"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-manylinux_2_24_s390x.whl", hash = "sha256:e0edd3c6762b3ff3fdbd90517a09808e5d67cce86d7c43ec6f5ca3f65bfe7fd9"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e76a9b0c2b2fb29a80764e106b1ea35c1b96a4e62e7ce7dde44f5df153fd5b66"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:88fc72e60d818924cb3d32948b682bcea0dadd0fd2efae9a4d0b7a55e310908a"},
+    {file = "pydantic_core-2.0.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:c04aa22ded4baf29c3c1ec3b76d5264dd91794b974a737251fdd0827abcc2c78"},
+    {file = "pydantic_core-2.0.1-cp39-none-win32.whl", hash = "sha256:4372e8fcb458aad1e155c04e663ff1840f36b859fb1422578372712a78866051"},
+    {file = "pydantic_core-2.0.1-cp39-none-win_amd64.whl", hash = "sha256:c5fef2dc7ed589ea83ac5ce526fcb8e8eb0ab79bfa67f958dafbda0a05ab3018"},
+    {file = "pydantic_core-2.0.1-pp37-pypy37_pp73-macosx_10_7_x86_64.whl", hash = "sha256:e4785a8c5440e410394f88e30c3db862ed05841595311ddc969b3fde377f95ea"},
+    {file = "pydantic_core-2.0.1-pp37-pypy37_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e90b99b6aa9fd6eee6d6f86921d38252c6e55c319dc6c5e411922d0dc173825"},
+    {file = "pydantic_core-2.0.1-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:182a0e5ce9382a0a77aab8407ead303b6e310c673a46b18937fa1a90c22ccbc4"},
+    {file = "pydantic_core-2.0.1-pp37-pypy37_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b83e11a68936f80ee92ef1001bf6b9fedf0602396acc417b16a9c136a9b3b7bd"},
+    {file = "pydantic_core-2.0.1-pp37-pypy37_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:5e4a918eeae2c566fdcad9ee89d8708a59dc5ec3d5083b61a886b19f82f69f5c"},
+    {file = "pydantic_core-2.0.1-pp37-pypy37_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:88b56a4e7480f4f22fa2faefdb0a887d70420d9cd8cb160677e8abe46769e7b0"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-macosx_10_7_x86_64.whl", hash = "sha256:3a85fde791e6567f879b50b59f1740afc55333060d93548d6bbb46bf1b6a1b49"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ef349e4ac794559c1538787a0fbce378a1beb991ef4f7707a6cde3156294259d"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f0f90928ed48b91d93add357fb1e81cef729bffaff3ab88882b76549434b4574"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:c3f8fea22690c6c33c4d36d2236732da29da560f815cd9aba1d3b5ab59dcb214"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:cbbefd38ef80b37d056592c366a164a37b4e87b12f0aba23c35087d890fb31ba"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:8945ba48644b45d4e66cc3e56b896e97fb1d7f166dd0ee1eb137bbfdf1285483"},
+    {file = "pydantic_core-2.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:1c318bd2bdaa88ec078dc7932e108a9c43caeabc84d2cf545081fb6a99ed1b90"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-macosx_10_7_x86_64.whl", hash = "sha256:7176ffa02c45d557cceb75f1290a2ddf53da680c6878aae54e69aafb21c52efd"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:176eb3ec03da4c36da7708d2398139e13d1130b3b3d1af4334a959f46278baa9"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:46bb28295082a22f3c7f5fa5546d669aed7eb43151ec0032e8c352c59f5e36af"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:e4b4c836100e5f07189b0aea8b4afae326f169bfdef91e86fd90a0d3c27f0c75"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-musllinux_1_1_aarch64.whl", hash = "sha256:b56f3758b82f26414a4dccd76f05c768df7bd2735e0ac43f3dfff2f5603d32a9"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-musllinux_1_1_x86_64.whl", hash = "sha256:0c8877d9e0bd128f103a1b0f02899aa7d4be1104eef5dc35e2b633042b64a2d1"},
+    {file = "pydantic_core-2.0.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:1672c8c36414c56adf704753b2d7e22e7528d7bd21cd357f24edeff76d4fd4ca"},
+    {file = "pydantic_core-2.0.1.tar.gz", hash = "sha256:f9fffcb5507bff84a1312d1616406cad157806f105d78bd184d1e6b3b00e6417"},
+]
+
+[package.dependencies]
+typing-extensions = [
+    {version = ">=4.6.0", markers = "platform_python_implementation != \"PyPy\""},
+    {version = ">=4.6.0,<4.7.0", markers = "platform_python_implementation == \"PyPy\""},
+]
 
 [[package]]
 name = "pytest"
 version = "7.3.0"
 description = "pytest: simple powerful testing with Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytest-7.3.0-py3-none-any.whl", hash = "sha256:933051fa1bfbd38a21e73c3960cebdad4cf59483ddba7696c48509727e17f201"},
     {file = "pytest-7.3.0.tar.gz", hash = "sha256:58ecc27ebf0ea643ebfdf7fb1249335da761a00c9f955bcd922349bcb68ee57d"},
 ]
 
@@ -587,15 +641,14 @@
 [package.extras]
 testing = ["argcomplete", "attrs (>=19.2.0)", "hypothesis (>=3.56)", "mock", "nose", "pygments (>=2.7.2)", "requests", "xmlschema"]
 
 [[package]]
 name = "pytest-asyncio"
 version = "0.20.3"
 description = "Pytest support for asyncio"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytest-asyncio-0.20.3.tar.gz", hash = "sha256:83cbf01169ce3e8eb71c6c278ccb0574d1a7a3bb8eaaf5e50e0ad342afb33b36"},
     {file = "pytest_asyncio-0.20.3-py3-none-any.whl", hash = "sha256:f129998b209d04fcc65c96fc85c11e5316738358909a8399e93be553d7656442"},
 ]
 
@@ -607,15 +660,14 @@
 docs = ["sphinx (>=5.3)", "sphinx-rtd-theme (>=1.0)"]
 testing = ["coverage (>=6.2)", "flaky (>=3.5.0)", "hypothesis (>=5.7.1)", "mypy (>=0.931)", "pytest-trio (>=0.7.0)"]
 
 [[package]]
 name = "pytest-cov"
 version = "4.0.0"
 description = "Pytest plugin for measuring coverage."
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "pytest-cov-4.0.0.tar.gz", hash = "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"},
     {file = "pytest_cov-4.0.0-py3-none-any.whl", hash = "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b"},
 ]
 
@@ -626,30 +678,28 @@
 [package.extras]
 testing = ["fields", "hunter", "process-tests", "pytest-xdist", "six", "virtualenv"]
 
 [[package]]
 name = "pytest-deadfixtures"
 version = "2.2.1"
 description = "A simple plugin to list unused fixtures in pytest"
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "pytest-deadfixtures-2.2.1.tar.gz", hash = "sha256:ca15938a4e8330993ccec9c6c847383d88b3cd574729530647dc6b492daa9c1e"},
     {file = "pytest_deadfixtures-2.2.1-py2.py3-none-any.whl", hash = "sha256:db71533f2d9456227084e00a1231e732973e299ccb7c37ab92e95032ab6c083e"},
 ]
 
 [package.dependencies]
 pytest = ">=3.0.0"
 
 [[package]]
 name = "pytest-mock"
 version = "3.10.0"
 description = "Thin-wrapper around the mock package for easier use with pytest"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytest-mock-3.10.0.tar.gz", hash = "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"},
     {file = "pytest_mock-3.10.0-py3-none-any.whl", hash = "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b"},
 ]
 
@@ -659,15 +709,14 @@
 [package.extras]
 dev = ["pre-commit", "pytest-asyncio", "tox"]
 
 [[package]]
 name = "pyyaml"
 version = "6.0"
 description = "YAML parser and emitter for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "PyYAML-6.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53"},
     {file = "PyYAML-6.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b"},
@@ -709,15 +758,14 @@
     {file = "PyYAML-6.0.tar.gz", hash = "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2"},
 ]
 
 [[package]]
 name = "questionary"
 version = "1.10.0"
 description = "Python library to build pretty command line user prompts ⭐️"
-category = "dev"
 optional = false
 python-versions = ">=3.6,<4.0"
 files = [
     {file = "questionary-1.10.0-py3-none-any.whl", hash = "sha256:fecfcc8cca110fda9d561cb83f1e97ecbb93c613ff857f655818839dac74ce90"},
     {file = "questionary-1.10.0.tar.gz", hash = "sha256:600d3aefecce26d48d97eee936fdb66e4bc27f934c3ab6dd1e292c4f43946d90"},
 ]
 
@@ -727,15 +775,14 @@
 [package.extras]
 docs = ["Sphinx (>=3.3,<4.0)", "sphinx-autobuild (>=2020.9.1,<2021.0.0)", "sphinx-autodoc-typehints (>=1.11.1,<2.0.0)", "sphinx-copybutton (>=0.3.1,<0.4.0)", "sphinx-rtd-theme (>=0.5.0,<0.6.0)"]
 
 [[package]]
 name = "ruff"
 version = "0.0.255"
 description = "An extremely fast Python linter, written in Rust."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "ruff-0.0.255-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:b2d71fb6a7e50501a2473864acffc85dee6b750c25db198f7e71fe1dbbff1aad"},
     {file = "ruff-0.0.255-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:6c97d746861a6010f941179e84bba9feb8a871815667471d9ed6beb98d45c252"},
     {file = "ruff-0.0.255-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9a7fa60085079b91a298b963361be9b1b1c724582af6c84be954cbabdbd9309a"},
     {file = "ruff-0.0.255-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:c089f7141496334ab5a127b54ce55e41f0d6714e68a4453a1e09d2204cdea8c3"},
@@ -754,66 +801,61 @@
     {file = "ruff-0.0.255.tar.gz", hash = "sha256:f9eb1d3b2eecbeedae419fa494c4e2a5e4484baf93a1ce0f81eddb005e1919c5"},
 ]
 
 [[package]]
 name = "termcolor"
 version = "2.2.0"
 description = "ANSI color formatting for output in terminal"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "termcolor-2.2.0-py3-none-any.whl", hash = "sha256:91ddd848e7251200eac969846cbae2dacd7d71c2871e92733289e7e3666f48e7"},
     {file = "termcolor-2.2.0.tar.gz", hash = "sha256:dfc8ac3f350788f23b2947b3e6cfa5a53b630b612e6cd8965a015a776020b99a"},
 ]
 
 [package.extras]
 tests = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "toml"
 version = "0.10.2"
 description = "Python Library for Tom's Obvious, Minimal Language"
-category = "dev"
 optional = false
 python-versions = ">=2.6, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
     {file = "toml-0.10.2-py2.py3-none-any.whl", hash = "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b"},
     {file = "toml-0.10.2.tar.gz", hash = "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"},
 ]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tomlkit"
 version = "0.11.7"
 description = "Style preserving TOML library"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomlkit-0.11.7-py3-none-any.whl", hash = "sha256:5325463a7da2ef0c6bbfefb62a3dc883aebe679984709aee32a317907d0a8d3c"},
     {file = "tomlkit-0.11.7.tar.gz", hash = "sha256:f392ef70ad87a672f02519f99967d28a4d3047133e2d1df936511465fbb3791d"},
 ]
 
 [[package]]
 name = "typed-ast"
 version = "1.5.4"
 description = "a fork of Python 2 and 3 ast modules with type comment support"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "typed_ast-1.5.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:669dd0c4167f6f2cd9f57041e03c3c2ebf9063d0757dc89f79ba1daa2bfca9d4"},
     {file = "typed_ast-1.5.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:211260621ab1cd7324e0798d6be953d00b74e0428382991adfddb352252f1d62"},
     {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:267e3f78697a6c00c689c03db4876dd1efdfea2f251a5ad6555e82a26847b4ac"},
     {file = "typed_ast-1.5.4-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:c542eeda69212fa10a7ada75e668876fdec5f856cd3d06829e6aa64ad17c8dfe"},
@@ -837,53 +879,61 @@
     {file = "typed_ast-1.5.4-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98f80dee3c03455e92796b58b98ff6ca0b2a6f652120c263efdba4d6c5e58f72"},
     {file = "typed_ast-1.5.4-cp39-cp39-win_amd64.whl", hash = "sha256:0fdbcf2fef0ca421a3f5912555804296f0b0960f0418c440f5d6d3abb549f3e1"},
     {file = "typed_ast-1.5.4.tar.gz", hash = "sha256:39e21ceb7388e4bb37f4c679d72707ed46c2fbf2a5609b8b8ebc4b067d977df2"},
 ]
 
 [[package]]
 name = "typing-extensions"
-version = "4.5.0"
+version = "4.6.3"
+description = "Backported and Experimental Type Hints for Python 3.7+"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
+    {file = "typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
+]
+
+[[package]]
+name = "typing-extensions"
+version = "4.7.1"
 description = "Backported and Experimental Type Hints for Python 3.7+"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
-    {file = "typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "wcwidth"
 version = "0.2.6"
 description = "Measures the displayed width of unicode strings in a terminal"
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {file = "wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
 
 [[package]]
 name = "zipp"
 version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
     {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [extras]
-all = ["pydantic"]
-pydantic = ["pydantic"]
+all = ["packaging", "pydantic"]
+pydantic = ["packaging", "pydantic"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
-content-hash = "2d8ea14ebe1151ac35b9546cf833be019a4aab51bbdc3c622a65b04191e634d9"
+content-hash = "7612dcc6b1282036c532e55280eff54549be96db2079fed41a3114dd4e3c709c"
```

### Comparing `casers-0.5.0/pyproject.toml` & `casers-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.5.0"
+version = "0.6.0"
 tag_format = "$version"
 version_files = [
     "casers/_version.py",
     "Cargo.toml:version",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "casers"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/casers"
 homepage = "https://pypi.org/project/casers"
 keywords = []
 
 [tool.poetry.scripts]
 casers = 'casers.cli.app:run'
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = {version = "^1", optional = true}
+pydantic = {version = ">=1", optional = true}
+packaging = {version = "^23.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 maturin = "^0.14.17"
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
@@ -40,16 +41,16 @@
 ruff = "^0.0.255"
 toml = "^0.10.2"
 
 [tool.poetry.group.git.dependencies]
 commitizen = "^2.42.1"
 
 [tool.poetry.extras]
-all = ["pydantic"]
-pydantic = ["pydantic"]
+all = ["pydantic", "packaging"]
+pydantic = ["pydantic", "packaging"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "casers"
```

### Comparing `casers-0.5.0/src/lib.rs` & `casers-0.6.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/tests/test_to_constant.py` & `casers-0.6.0/tests/test_to_constant.py`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/tests/test_to_kebab.py` & `casers-0.6.0/tests/test_to_kebab.py`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/tests/test_to_snake.py` & `casers-0.6.0/tests/test_to_snake.py`

 * *Files identical despite different names*

### Comparing `casers-0.5.0/Cargo.lock` & `casers-0.6.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "casers"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
```

### Comparing `casers-0.5.0/PKG-INFO` & `casers-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: casers
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/daxartio/casers
 Project-URL: homepage, https://pypi.org/project/casers
+Project-URL: repository, https://github.com/daxartio/casers
 
 # casers
 
 [![PyPI](https://img.shields.io/pypi/v/casers)](https://pypi.org/project/casers/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/casers)](https://www.python.org/downloads/)
 [![GitHub last commit](https://img.shields.io/github/last-commit/daxartio/casers)](https://github.com/daxartio/casers)
 [![GitHub stars](https://img.shields.io/github/stars/daxartio/casers?style=social)](https://github.com/daxartio/casers)
@@ -59,23 +59,27 @@
 >>> to_kebab("someText") == "some-text"
 True
 >>> to_kebab("some_text") == "some-text"
 True
 
 ```
 
+### pydantic
+
+The package supports for pydantic 1 and 2 versions
+
 ```python
 >>> from casers.pydantic import CamelAliases
 
 >>> class Model(CamelAliases):
 ...     snake_case: str
 
->>> Model.parse_obj({"snakeCase": "value"}).snake_case == "value"
+>>> Model.model_validate({"snakeCase": "value"}).snake_case == "value"
 True
->>> Model.parse_raw('{"snakeCase": "value"}').snake_case == "value"
+>>> Model.model_validate_json('{"snakeCase": "value"}').snake_case == "value"
 True
 
 ```
 
 ## License
 
 * [MIT LICENSE](LICENSE)
```

