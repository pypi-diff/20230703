# Comparing `tmp/not_again_ai-0.1.5.tar.gz` & `tmp/not_again_ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_again_ai-0.1.5.tar", max compression
+gzip compressed data, was "not_again_ai-0.1.6.tar", max compression
```

## Comparing `not_again_ai-0.1.5.tar` & `not_again_ai-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-02-04 21:52:11.091766 not_again_ai-0.1.5/LICENSE
--rw-r--r--   0        0        0    13592 2023-02-04 21:57:48.190699 not_again_ai-0.1.5/README.md
--rw-r--r--   0        0        0     4052 2023-02-05 00:39:16.553529 not_again_ai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/__init__.py
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/data_analysis/__init__.py
--rw-r--r--   0        0        0     4488 2022-11-20 17:31:57.604401 not_again_ai-0.1.5/src/not_again_ai/data_analysis/dependence.py
--rw-r--r--   0        0        0     3424 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/parallel.py
--rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/py.typed
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/system/__init__.py
--rw-r--r--   0        0        0      344 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/system/files.py
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/viz/__init__.py
--rw-r--r--   0        0        0     3340 2023-02-05 00:34:30.555034 not_again_ai-0.1.5/src/not_again_ai/viz/barplots.py
--rw-r--r--   0        0        0     4413 2022-11-20 17:31:57.600401 not_again_ai-0.1.5/src/not_again_ai/viz/distributions.py
--rw-r--r--   0        0        0     2337 2022-11-20 17:31:57.588401 not_again_ai-0.1.5/src/not_again_ai/viz/scatterplot.py
--rw-r--r--   0        0        0     5153 2022-11-20 17:31:57.600401 not_again_ai-0.1.5/src/not_again_ai/viz/time_series.py
--rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.1.5/src/not_again_ai/viz/utils.py
--rw-r--r--   0        0        0    15113 1970-01-01 00:00:00.000000 not_again_ai-0.1.5/setup.py
--rw-r--r--   0        0        0    15059 1970-01-01 00:00:00.000000 not_again_ai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-02-04 21:52:11.091766 not_again_ai-0.1.6/LICENSE
+-rw-r--r--   0        0        0    13426 2023-07-03 19:45:21.082944 not_again_ai-0.1.6/README.md
+-rw-r--r--   0        0        0     3980 2023-07-03 17:00:52.280650 not_again_ai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/data_analysis/__init__.py
+-rw-r--r--   0        0        0     4488 2022-11-20 17:31:57.604401 not_again_ai-0.1.6/src/not_again_ai/data_analysis/dependence.py
+-rw-r--r--   0        0        0     3424 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/parallel.py
+-rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/py.typed
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/system/__init__.py
+-rw-r--r--   0        0        0      344 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/system/files.py
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/viz/__init__.py
+-rw-r--r--   0        0        0     3340 2023-02-05 00:34:30.555034 not_again_ai-0.1.6/src/not_again_ai/viz/barplots.py
+-rw-r--r--   0        0        0     4413 2023-07-03 19:40:40.547380 not_again_ai-0.1.6/src/not_again_ai/viz/distributions.py
+-rw-r--r--   0        0        0     2337 2023-07-03 16:51:29.949602 not_again_ai-0.1.6/src/not_again_ai/viz/scatterplot.py
+-rw-r--r--   0        0        0     5153 2022-11-20 17:31:57.600401 not_again_ai-0.1.6/src/not_again_ai/viz/time_series.py
+-rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.1.6/src/not_again_ai/viz/utils.py
+-rw-r--r--   0        0        0    14973 1970-01-01 00:00:00.000000 not_again_ai-0.1.6/setup.py
+-rw-r--r--   0        0        0    14920 1970-01-01 00:00:00.000000 not_again_ai-0.1.6/PKG-INFO
```

### Comparing `not_again_ai-0.1.5/LICENSE` & `not_again_ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/README.md` & `not_again_ai-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # not-again-ai
 
-[![GitHub Actions][github-actions-badge]](https://github.com/DaveCoDev/not-again-ai/actions)
+[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)
 [![Packaged with Poetry][poetry-badge]](https://python-poetry.org/)
-[![Code style: black][black-badge]](https://github.com/psf/black)
-[![Imports: isort][isort-badge]](https://pycqa.github.io/isort/)
+[![Nox][nox-badge]](https://github.com/wntrblm/nox)
+[![Code style: Black][black-badge]](https://github.com/psf/black)
+[![Ruff][ruff-badge]](https://github.com/astral-sh/ruff)
 [![Type checked with mypy][mypy-badge]](https://mypy-lang.org/)
 
-[github-actions-badge]: https://github.com/DaveCoDev/not-again-ai/workflows/python/badge.svg
+[github-actions-badge]: https://github.com/johnthagen/python-blueprint/workflows/python/badge.svg
+[poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg
+[nox-badge]: https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[isort-badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[ruff-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
 [mypy-badge]: https://www.mypy-lang.org/static/mypy_badge.svg
-[poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg
 
 Have you ever been working on a project and groaned as you go to search again on how to nicely plot a simple distribution? Or have you been frustrated at wanting to run multiple functions in parallel, but stuck between the seemingly ten different ways to do it?
 **not-again-ai** is a Python package designed to once and for all collect all these little things that come up over and over again in AI projects and put them in one place.
 
 **Documentation** available at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).
 
 # Installation
@@ -98,15 +100,15 @@
 
 # Development Information
 
 This package uses [Poetry](https://python-poetry.org/) to manage dependencies and
 isolated [Python virtual environments](https://docs.python.org/3/library/venv.html).
 
 To proceed, 
-[install Poetry globally onto your system](https://python-poetry.org/docs/#installation).
+[install Poetry globally onto your system](https://python-poetry.org/docs/#installing-with-the-official-installer).
 
 (Optional) configure Poetry to use an in-project virtual environment.
 ```bash
 $ poetry config virtualenvs.in-project true
 ```
 
 ## Dependencies
@@ -132,15 +134,15 @@
 
 To deactivate the environment:
 
 ```bash
 (.venv) $ exit
 ```
 
-To upgrade all dependencies to their latest versions:
+To upgrade all dependencies to the versions defined in [`pyproject.toml`](./pyproject.toml):
 
 ```bash
 $ poetry update
 ```
 
 ## Packaging
 
@@ -155,15 +157,15 @@
 [source distribution](https://packaging.python.org/en/latest/flow/#the-source-distribution-sdist) and
 a [wheel](https://packaging.python.org/en/latest/specifications/binary-distribution-format/):
 
 ```bash
 $ poetry build
 ```
 
-This will generate `dist/not-again-ai-0.1.0.tar.gz` and `dist/not_again_ai-0.1.0-py3-none-any.whl`.
+This will generate `dist/not-again-ai-<version>.tar.gz` and `dist/not_again_ai-<version>-py3-none-any.whl`.
 
 Read more about the [advantages of wheels](https://pythonwheels.com/) to understand why generating
 wheel distributions are important.
 
 ## Publish Distributions to PyPI
 
 Source and wheel redistributable packages can
@@ -222,37 +224,33 @@
 ```bash
 (.venv) $ nox -s test -- -k invalid_factorial
 ```
 
 ## Code Style Checking
 
 [PEP 8](https://peps.python.org/pep-0008/) is the universally accepted style guide for
-Python code. PEP 8 code compliance is verified using [Flake8](http://flake8.pycqa.org/). Flake8 is
-configured in the `[tool.flake8]` section of `pyproject.toml`. Extra Flake8 plugins are also
-included:
-
-- `flake8-bugbear`: Find likely bugs and design problems in your program.
-- `flake8-broken-line`: Forbid using backslashes (`\`) for line breaks.
-- `flake8-comprehensions`: Helps write better `list`/`set`/`dict` comprehensions.
-- `pep8-naming`: Ensure functions, classes, and variables are named with correct casing.
-- `flake8-pyproject`: Allow configuration of `flake8` through `pyproject.toml`.
-
-Some code style settings are included in [`.editorconfig`](./.editorconfig) and will be
-configured automatically in editors such as PyCharm.
+Python code. PEP 8 code compliance is verified using [Ruff](https://github.com/astral-sh/ruff).
+Ruff is configured in the `[tool.ruff]` section of `pyproject.toml`.
 
 To lint code, run:
 
 ```bash
 (.venv) $ nox -s lint
 ```
 
+To automatically fix fixable lint errors, run:
+
+```bash
+(.venv) $ nox -s lint_fix
+```
+
 ## Automated Code Formatting
 
 Code is automatically formatted using [black](https://github.com/psf/black). Imports are
-automatically sorted and grouped using [isort](https://github.com/PyCQA/isort/).
+automatically sorted and grouped using [Ruff](https://github.com/astral-sh/ruff).
 
 These tools are configured by:
 
 - [`pyproject.toml`](./pyproject.toml)
 
 To automatically format code, run:
 
@@ -305,15 +303,17 @@
 
 GitHub Actions is configured in [`.github/workflows/python.yml`](./.github/workflows/python.yml).
 
 ## [Visual Studio Code](https://code.visualstudio.com/docs/languages/python)
 
 Install the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VSCode.
 
-Default settings are configured in [`.vscode/settings.json`](./.vscode/settings.json). This will enable flake8 and black formatting with consistent settings.
+Install the [Ruff extension](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff) for VSCode.
+
+Default settings are configured in [`.vscode/settings.json`](./.vscode/settings.json). This will enable Ruff and black with consistent settings.
 
 # Documentation
 
 ## Generating a User Guide
 
 [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) is a powerful static site
 generator that combines easy-to-write Markdown, with a number of Markdown extensions that increase
```

### Comparing `not_again_ai-0.1.5/pyproject.toml` & `not_again_ai-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "not-again-ai"
-version = "0.1.5"
+version = "0.1.6"
 description = "Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place."
 authors = ["DaveCoDev <dave.co.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaveCoDev/not-again-ai"
 documentation = "https://github.com/DaveCoDev/not-again-ai"
 classifiers = [
@@ -18,103 +18,103 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 
-
 [tool.poetry.dependencies]
 # Some packages, such as scipy, constrain their upper bound of Python versions they support.
 # Without also constraining the upper bound here, Poetry will not select those versions and will
 # result in an old version being resolved/locked.
 python = "^3.9, <3.12"
-numpy = "^1.22.4"
-pandas = "^1.4.2"
-seaborn = "^0"
-scipy = "^1"
-scikit-learn = "^1"
+numpy = "^1.25.0"
+pandas = "^2.0.3"
+seaborn = "^0.12.2"
+scipy = "^1.11.1"
+scikit-learn = "^1.3.0"
 
 [tool.poetry.group.nox.dependencies]
 nox-poetry = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pytest-cov = "*"
 
 [tool.poetry.group.type_check.dependencies]
 mypy = "*"
 # As of mypy 0.900, mypy no longer bundles the stubs for third-party libraries that reside
 # in the typeshed project. Add these "types-" packages here if you depend on them in
 # requirements.in (e.g. types-requests).
 # See: http://mypy-lang.blogspot.com/2021/06/mypy-0900-released.html
-#      https://github.com/python/typeshed/tree/master/stubs
+#      https://github.com/python/typeshed/tree/main/stubs
 
 [tool.poetry.group.lint.dependencies]
-flake8 = "*"
-flake8-bugbear = "*"
-flake8-broken-line = "*"
-flake8-comprehensions = "*"
-pep8-naming = "*"
-# TODO: Remove this when flake8 adds native support for pyproject.toml.
-flake8-pyproject = "*"
+ruff = "*"
 
 [tool.poetry.group.fmt.dependencies]
 black = "*"
-isort = "*"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "*"
 mkdocs-htmlproofer-plugin = "*"
 mkdocstrings = { version = "*", extras = ["python"] }
 ## Autodoc.
 mkdocs-gen-files = "*"
 mkdocs-literate-nav = "*"
 
-
 [tool.poetry.scripts]
 not-again-ai = "not_again_ai.cli:entry_point"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
 # If certain strict config options are too pedantic for a project,
 # disable them selectively here by setting to false.
 
-# Note: This configuration is supported by flake8-pyproject.
-[tool.flake8]
-max-line-length = 120
-# This ignore is required by black.
-extend-ignore = "E203,E501"
+[tool.ruff]
+line-length = 120
+target-version = "py38"
+extend-select = [
+    "I", # isort
+    "N", # pep8-naming
+    "UP", # pyupgrade
+    "RUF", # ruff
+    "B", # flake8-bugbear
+    "C4", # flake8-comprehensions
+    "PTH", # flake8-use-pathlib
+    "SIM", # flake8-simplify
+    "TID", # flake8-tidy-imports
+]
+extend-ignore = ["RUF005", "E501"]
+src = ["src"]
+
+[tool.ruff.isort]
+force-sort-within-sections = true
+split-on-trailing-comma = false
+# For non-src directory projects, explicitly set top level package names:
+# known-first-party = ["my-app"]
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.flake8-bugbear]
+extend-immutable-calls = ["typer.Argument"]
 
 [tool.black]
 line-length = 120
 target-version = ["py39", "py310", "py311"]
 # black will automatically exclude all files listed in .gitignore
 # If you need to exclude additional folders, consider using extend-exclude to avoid disabling the
 # default .gitignore behaviour.
 
-
-[tool.isort]
-profile = "black"
-line_length = 120
-force_sort_within_sections = true
-# Inform isort of paths to import names that should be considered part of the "First Party" group.
-src_paths = ["src/not_again_ai"]
-skip_gitignore = true
-# If you need to skip/exclude folders, consider using skip_glob as that will allow the
-# isort defaults for skip to remain without the need to duplicate them.
-
-
 [tool.pytest.ini_options]
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
 xfail_strict = true
 filterwarnings = [
@@ -122,10 +122,9 @@
     # See: https://docs.pytest.org/en/latest/reference/reference.html#confval-filterwarnings
     "error",
     # Add additional warning supressions as needed here. For example, if a third-party library
     # is throwing a deprecation warning that needs to be fixed upstream:
     # "ignore::DeprecationWarning:typer",
 ]
 
-
 [tool.coverage.run]
-branch = true
+branch = true
```

### Comparing `not_again_ai-0.1.5/src/not_again_ai/data_analysis/dependence.py` & `not_again_ai-0.1.6/src/not_again_ai/data_analysis/dependence.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/src/not_again_ai/parallel.py` & `not_again_ai-0.1.6/src/not_again_ai/parallel.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/src/not_again_ai/viz/barplots.py` & `not_again_ai-0.1.6/src/not_again_ai/viz/barplots.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/src/not_again_ai/viz/distributions.py` & `not_again_ai-0.1.6/src/not_again_ai/viz/distributions.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/src/not_again_ai/viz/scatterplot.py` & `not_again_ai-0.1.6/src/not_again_ai/viz/scatterplot.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/src/not_again_ai/viz/time_series.py` & `not_again_ai-0.1.6/src/not_again_ai/viz/time_series.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.1.5/setup.py` & `not_again_ai-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,28 @@
  'not_again_ai.system',
  'not_again_ai.viz']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.22.4,<2.0.0',
- 'pandas>=1.4.2,<2.0.0',
- 'scikit-learn>=1,<2',
- 'scipy>=1,<2',
- 'seaborn>=0,<1']
+['numpy>=1.25.0,<2.0.0',
+ 'pandas>=2.0.3,<3.0.0',
+ 'scikit-learn>=1.3.0,<2.0.0',
+ 'scipy>=1.11.1,<2.0.0',
+ 'seaborn>=0.12.2,<0.13.0']
 
 entry_points = \
 {'console_scripts': ['not-again-ai = not_again_ai.cli:entry_point']}
 
 setup_kwargs = {
     'name': 'not-again-ai',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.',
-    'long_description': '# not-again-ai\n\n[![GitHub Actions][github-actions-badge]](https://github.com/DaveCoDev/not-again-ai/actions)\n[![Packaged with Poetry][poetry-badge]](https://python-poetry.org/)\n[![Code style: black][black-badge]](https://github.com/psf/black)\n[![Imports: isort][isort-badge]](https://pycqa.github.io/isort/)\n[![Type checked with mypy][mypy-badge]](https://mypy-lang.org/)\n\n[github-actions-badge]: https://github.com/DaveCoDev/not-again-ai/workflows/python/badge.svg\n[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg\n[isort-badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336\n[mypy-badge]: https://www.mypy-lang.org/static/mypy_badge.svg\n[poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg\n\nHave you ever been working on a project and groaned as you go to search again on how to nicely plot a simple distribution? Or have you been frustrated at wanting to run multiple functions in parallel, but stuck between the seemingly ten different ways to do it?\n**not-again-ai** is a Python package designed to once and for all collect all these little things that come up over and over again in AI projects and put them in one place.\n\n**Documentation** available at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).\n\n# Installation\n\nRequires: Python 3.9, 3.10, or 3.11\n\nInstall from [PyPI](https://pypi.org/project/not-again-ai/)\n\n```bash\n$ pip install not_again_ai\n```\n\n# Quick tour\n\n## Visualization\n\nWe currently offer two visualization tools, a time series plot and a histogram for plotting univariate distributions.\n\n```python\n>>> import numpy as np\n>>> import pandas as pd\n>>> from not_again_ai.viz.time_series import ts_lineplot\n>>> from not_again_ai.viz.distributions import univariate_distplot\n\n# get some time series data\n>>> rs = np.random.RandomState(365)\n>>> values = rs.randn(365, 4).cumsum(axis=0)\n>>> dates = pd.date_range(\'1 1 2021\', periods=365, freq=\'D\')\n# plot the time series and save it to a file\n>>> ts_lineplot(ts_data=values, save_pathname=\'myplot.png\', ts_x=dates, ts_names=[\'A\', \'B\', \'C\', \'D\'])\n\n# get a random distribution\n>>> distrib = np.random.beta(a=0.5, b=0.5, size=1000)\n# plot the distribution and save it to a file\n>>> univariate_distplot(\n...     data=distrib, \n...     save_pathname=\'mydistribution.svg\', \n...     print_summary=False, bins=100, \n...     title=r\'Beta Distribution $\\alpha=0.5, \\beta=0.5$\'\n... )\n```\n\n<p float="center">\n  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/distributions_test4.svg" width="404" />\n  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/ts_lineplot5.svg" width="404" /> \n</p>\n\n## Parallel\nFor when you have functions you want to execute in parallel.\n\n```python\n# execute the passed in functions in parallel without any additional arguments\n>>> result = embarrassingly_parallel_simple([do_something, do_something2], num_processes=2)\n\n# execute the function mult in parallel with the passed in arguments\n>>> args = ((2, 2), (3, 3), (4, 4))\n>>> result2 = embarrassingly_parallel(mult, args, num_processes=multiprocessing.cpu_count())\n```\n\n## Filesystem\nWe provide helpers to deal with files and directories easily and without raising unnecessary errors.\n\n```python\n>>> from not_again_ai.system.files import create_file_dir\n\n# creates the directory mydir if it does not exist\n>>> create_file_dir(\'mydir/myfile.txt\')\n```\n\n## Data Analysis\nWe provide a few helpers for data analysis.\n\n```python\nfrom not_again_ai.data_analysis.dependence import pearson_correlation\n# quadratic dependence\n>>> x = (rs.rand(500) * 4) - 2\n>>> y = x**2 + (rs.randn(500) * 0.2)\n>>> pearson_correlation(x, y)\n0.05\n```\n\n# Development Information\n\nThis package uses [Poetry](https://python-poetry.org/) to manage dependencies and\nisolated [Python virtual environments](https://docs.python.org/3/library/venv.html).\n\nTo proceed, \n[install Poetry globally onto your system](https://python-poetry.org/docs/#installation).\n\n(Optional) configure Poetry to use an in-project virtual environment.\n```bash\n$ poetry config virtualenvs.in-project true\n```\n\n## Dependencies\n\nDependencies are defined in [`pyproject.toml`](./pyproject.toml) and specific versions are locked\ninto [`poetry.lock`](./poetry.lock). This allows for exact reproducible environments across\nall machines that use the project, both during development and in production.\n\nTo install all dependencies into an isolated virtual environment:\n\n> Append `--sync` to uninstall dependencies that are no longer in use from the virtual environment.\n\n```bash\n$ poetry install\n```\n\nTo [activate](https://python-poetry.org/docs/basic-usage#activating-the-virtual-environment) the\nvirtual environment that is automatically created by Poetry:\n\n```bash\n$ poetry shell\n```\n\nTo deactivate the environment:\n\n```bash\n(.venv) $ exit\n```\n\nTo upgrade all dependencies to their latest versions:\n\n```bash\n$ poetry update\n```\n\n## Packaging\n\nThis project is designed as a Python package, meaning that it can be bundled up and redistributed\nas a single compressed file.\n\nPackaging is configured by:\n\n- [`pyproject.toml`](./pyproject.toml)\n\nTo package the project as both a \n[source distribution](https://packaging.python.org/en/latest/flow/#the-source-distribution-sdist) and\na [wheel](https://packaging.python.org/en/latest/specifications/binary-distribution-format/):\n\n```bash\n$ poetry build\n```\n\nThis will generate `dist/not-again-ai-0.1.0.tar.gz` and `dist/not_again_ai-0.1.0-py3-none-any.whl`.\n\nRead more about the [advantages of wheels](https://pythonwheels.com/) to understand why generating\nwheel distributions are important.\n\n## Publish Distributions to PyPI\n\nSource and wheel redistributable packages can\nbe [published to PyPI](https://python-poetry.org/docs/cli#publish) or installed\ndirectly from the filesystem using `pip`.\n\n```bash\n$ poetry publish\n```\n\n# Enforcing Code Quality\n\nAutomated code quality checks are performed using \n[Nox](https://nox.thea.codes/en/stable/) and\n[`nox-poetry`](https://nox-poetry.readthedocs.io/en/stable/). Nox will automatically create virtual\nenvironments and run commands based on [`noxfile.py`](./noxfile.py) for unit testing, PEP 8 style\nguide checking, type checking and documentation generation.\n\n> Note: `nox` is installed into the virtual environment automatically by the `poetry install`\n> command above. Run `poetry shell` to activate the virtual environment.\n\nTo run all default sessions:\n\n```bash\n(.venv) $ nox\n```\n\n## Unit Testing\n\nUnit testing is performed with [pytest](https://pytest.org/). pytest has become the de facto Python\nunit testing framework. Some key advantages over the built-in\n[unittest](https://docs.python.org/3/library/unittest.html) module are:\n\n1. Significantly less boilerplate needed for tests.\n2. PEP 8 compliant names (e.g. `pytest.raises()` instead of `self.assertRaises()`).\n3. Vibrant ecosystem of plugins.\n\npytest will automatically discover and run tests by recursively searching for folders and `.py`\nfiles prefixed with `test` for any functions prefixed by `test`.\n\nThe `tests` folder is created as a Python package (i.e. there is an `__init__.py` file within it)\nbecause this helps `pytest` uniquely namespace the test files. Without this, two test files cannot\nbe named the same, even if they are in different subdirectories.\n\nCode coverage is provided by the [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/) plugin.\n\nWhen running a unit test Nox session (e.g. `nox -s test`), an HTML report is generated in\nthe `htmlcov` folder showing each source file and which lines were executed during unit testing.\nOpen `htmlcov/index.html` in a web browser to view the report. Code coverage reports help identify\nareas of the project that are currently not tested.\n\npytest and code coverage are configured in [`pyproject.toml`](./pyproject.toml).\n\nTo pass arguments to `pytest` through `nox`:\n\n```bash\n(.venv) $ nox -s test -- -k invalid_factorial\n```\n\n## Code Style Checking\n\n[PEP 8](https://peps.python.org/pep-0008/) is the universally accepted style guide for\nPython code. PEP 8 code compliance is verified using [Flake8](http://flake8.pycqa.org/). Flake8 is\nconfigured in the `[tool.flake8]` section of `pyproject.toml`. Extra Flake8 plugins are also\nincluded:\n\n- `flake8-bugbear`: Find likely bugs and design problems in your program.\n- `flake8-broken-line`: Forbid using backslashes (`\\`) for line breaks.\n- `flake8-comprehensions`: Helps write better `list`/`set`/`dict` comprehensions.\n- `pep8-naming`: Ensure functions, classes, and variables are named with correct casing.\n- `flake8-pyproject`: Allow configuration of `flake8` through `pyproject.toml`.\n\nSome code style settings are included in [`.editorconfig`](./.editorconfig) and will be\nconfigured automatically in editors such as PyCharm.\n\nTo lint code, run:\n\n```bash\n(.venv) $ nox -s lint\n```\n\n## Automated Code Formatting\n\nCode is automatically formatted using [black](https://github.com/psf/black). Imports are\nautomatically sorted and grouped using [isort](https://github.com/PyCQA/isort/).\n\nThese tools are configured by:\n\n- [`pyproject.toml`](./pyproject.toml)\n\nTo automatically format code, run:\n\n```bash\n(.venv) $ nox -s fmt\n```\n\nTo verify code has been formatted, such as in a CI job:\n\n```bash\n(.venv) $ nox -s fmt_check\n```\n\n## Type Checking\n\n[Type annotations](https://docs.python.org/3/library/typing.html) allows developers to include\noptional static typing information to Python source code. This allows static analyzers such\nas [mypy](http://mypy-lang.org/), [PyCharm](https://www.jetbrains.com/pycharm/),\nor [Pyright](https://github.com/microsoft/pyright) to check that functions are used with the\ncorrect types before runtime.\n\n\n```python\ndef factorial(n: int) -> int:\n    ...\n```\n\nmypy is configured in [`pyproject.toml`](./pyproject.toml). To type check code, run:\n\n```bash\n(.venv) $ nox -s type_check\n```\n\nSee also [awesome-python-typing](https://github.com/typeddjango/awesome-python-typing).\n\n### Distributing Type Annotations\n\n[PEP 561](https://www.python.org/dev/peps/pep-0561/) defines how a Python package should\ncommunicate the presence of inline type annotations to static type\ncheckers. [mypy\'s documentation](https://mypy.readthedocs.io/en/stable/installed_packages.html)\nprovides further examples on how to do this.\n\nMypy looks for the existence of a file named [`py.typed`](./src/not-again-ai/py.typed) in the root of the\ninstalled package to indicate that inline type annotations should be checked.\n\n## Continuous Integration\n\nContinuous integration is provided by [GitHub Actions](https://github.com/features/actions). This\nruns all tests, lints, and type checking for every commit and pull request to the repository.\n\nGitHub Actions is configured in [`.github/workflows/python.yml`](./.github/workflows/python.yml).\n\n## [Visual Studio Code](https://code.visualstudio.com/docs/languages/python)\n\nInstall the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VSCode.\n\nDefault settings are configured in [`.vscode/settings.json`](./.vscode/settings.json). This will enable flake8 and black formatting with consistent settings.\n\n# Documentation\n\n## Generating a User Guide\n\n[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) is a powerful static site\ngenerator that combines easy-to-write Markdown, with a number of Markdown extensions that increase\nthe power of Markdown. This makes it a great fit for user guides and other technical documentation.\n\nThe example MkDocs project included in this project is configured to allow the built documentation\nto be hosted at any URL or viewed offline from the file system.\n\nTo build the user guide, run,\n\n```bash\n(.venv) $ nox -s docs\n```\n\nand open `docs/user_guide/site/index.html` using a web browser.\n\nTo build the user guide, additionally validating external URLs, run:\n\n```bash\n(.venv) $ nox -s docs_check_urls\n```\n\nTo build the user guide in a format suitable for viewing directly from the file system, run:\n\n```bash\n(.venv) $ nox -s docs_offline\n```\n\nTo build and serve the user guide with automatic rebuilding as you change the contents,\nrun:\n\n```bash\n(.venv) $ nox -s docs_serve\n``` \n\nand open <http://127.0.0.1:8000> in a browser.\n\nEach time the `main` Git branch is updated, the \n[`.github/workflows/pages.yml`](.github/workflows/pages.yml) GitHub Action will\nautomatically build the user guide and publish it to [GitHub Pages](https://pages.github.com/).\nThis is configured in the `docs_github_pages` Nox session.\n\n## Generating API Documentation\n\nThis project uses [mkdocstrings](https://github.com/mkdocstrings/mkdocstrings) plugin for\nMkDocs, which renders\n[Google-style docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)\ninto an MkDocs project. Google-style docstrings provide a good mix of easy-to-read docstrings in\ncode as well as nicely-rendered output.\n\n```python\n"""Computes the factorial through a recursive algorithm.\n\nArgs:\n    n: A positive input value.\n\nRaises:\n    InvalidFactorialError: If n is less than 0.\n\nReturns:\n    Computed factorial.\n"""\n```\n\n## Misc\n\nIf you get a `Failed to create the collection: Prompt dismissed..` error when running `poetry update` on Ubuntu, try setting the following environment variable:\n\n    ```bash\n    export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring\n    ```\n\n# Attributions\n[python-blueprint](https://github.com/johnthagen/python-blueprint) for the Python package skeleton.\n',
+    'long_description': '# not-again-ai\n\n[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)\n[![Packaged with Poetry][poetry-badge]](https://python-poetry.org/)\n[![Nox][nox-badge]](https://github.com/wntrblm/nox)\n[![Code style: Black][black-badge]](https://github.com/psf/black)\n[![Ruff][ruff-badge]](https://github.com/astral-sh/ruff)\n[![Type checked with mypy][mypy-badge]](https://mypy-lang.org/)\n\n[github-actions-badge]: https://github.com/johnthagen/python-blueprint/workflows/python/badge.svg\n[poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg\n[nox-badge]: https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg\n[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg\n[ruff-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json\n[mypy-badge]: https://www.mypy-lang.org/static/mypy_badge.svg\n\nHave you ever been working on a project and groaned as you go to search again on how to nicely plot a simple distribution? Or have you been frustrated at wanting to run multiple functions in parallel, but stuck between the seemingly ten different ways to do it?\n**not-again-ai** is a Python package designed to once and for all collect all these little things that come up over and over again in AI projects and put them in one place.\n\n**Documentation** available at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).\n\n# Installation\n\nRequires: Python 3.9, 3.10, or 3.11\n\nInstall from [PyPI](https://pypi.org/project/not-again-ai/)\n\n```bash\n$ pip install not_again_ai\n```\n\n# Quick tour\n\n## Visualization\n\nWe currently offer two visualization tools, a time series plot and a histogram for plotting univariate distributions.\n\n```python\n>>> import numpy as np\n>>> import pandas as pd\n>>> from not_again_ai.viz.time_series import ts_lineplot\n>>> from not_again_ai.viz.distributions import univariate_distplot\n\n# get some time series data\n>>> rs = np.random.RandomState(365)\n>>> values = rs.randn(365, 4).cumsum(axis=0)\n>>> dates = pd.date_range(\'1 1 2021\', periods=365, freq=\'D\')\n# plot the time series and save it to a file\n>>> ts_lineplot(ts_data=values, save_pathname=\'myplot.png\', ts_x=dates, ts_names=[\'A\', \'B\', \'C\', \'D\'])\n\n# get a random distribution\n>>> distrib = np.random.beta(a=0.5, b=0.5, size=1000)\n# plot the distribution and save it to a file\n>>> univariate_distplot(\n...     data=distrib, \n...     save_pathname=\'mydistribution.svg\', \n...     print_summary=False, bins=100, \n...     title=r\'Beta Distribution $\\alpha=0.5, \\beta=0.5$\'\n... )\n```\n\n<p float="center">\n  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/distributions_test4.svg" width="404" />\n  <img src="https://raw.githubusercontent.com/DaveCoDev/not-again-ai/44c53fb7fb07234aaceea40c90d8cb74e5fa6c15/assets/ts_lineplot5.svg" width="404" /> \n</p>\n\n## Parallel\nFor when you have functions you want to execute in parallel.\n\n```python\n# execute the passed in functions in parallel without any additional arguments\n>>> result = embarrassingly_parallel_simple([do_something, do_something2], num_processes=2)\n\n# execute the function mult in parallel with the passed in arguments\n>>> args = ((2, 2), (3, 3), (4, 4))\n>>> result2 = embarrassingly_parallel(mult, args, num_processes=multiprocessing.cpu_count())\n```\n\n## Filesystem\nWe provide helpers to deal with files and directories easily and without raising unnecessary errors.\n\n```python\n>>> from not_again_ai.system.files import create_file_dir\n\n# creates the directory mydir if it does not exist\n>>> create_file_dir(\'mydir/myfile.txt\')\n```\n\n## Data Analysis\nWe provide a few helpers for data analysis.\n\n```python\nfrom not_again_ai.data_analysis.dependence import pearson_correlation\n# quadratic dependence\n>>> x = (rs.rand(500) * 4) - 2\n>>> y = x**2 + (rs.randn(500) * 0.2)\n>>> pearson_correlation(x, y)\n0.05\n```\n\n# Development Information\n\nThis package uses [Poetry](https://python-poetry.org/) to manage dependencies and\nisolated [Python virtual environments](https://docs.python.org/3/library/venv.html).\n\nTo proceed, \n[install Poetry globally onto your system](https://python-poetry.org/docs/#installing-with-the-official-installer).\n\n(Optional) configure Poetry to use an in-project virtual environment.\n```bash\n$ poetry config virtualenvs.in-project true\n```\n\n## Dependencies\n\nDependencies are defined in [`pyproject.toml`](./pyproject.toml) and specific versions are locked\ninto [`poetry.lock`](./poetry.lock). This allows for exact reproducible environments across\nall machines that use the project, both during development and in production.\n\nTo install all dependencies into an isolated virtual environment:\n\n> Append `--sync` to uninstall dependencies that are no longer in use from the virtual environment.\n\n```bash\n$ poetry install\n```\n\nTo [activate](https://python-poetry.org/docs/basic-usage#activating-the-virtual-environment) the\nvirtual environment that is automatically created by Poetry:\n\n```bash\n$ poetry shell\n```\n\nTo deactivate the environment:\n\n```bash\n(.venv) $ exit\n```\n\nTo upgrade all dependencies to the versions defined in [`pyproject.toml`](./pyproject.toml):\n\n```bash\n$ poetry update\n```\n\n## Packaging\n\nThis project is designed as a Python package, meaning that it can be bundled up and redistributed\nas a single compressed file.\n\nPackaging is configured by:\n\n- [`pyproject.toml`](./pyproject.toml)\n\nTo package the project as both a \n[source distribution](https://packaging.python.org/en/latest/flow/#the-source-distribution-sdist) and\na [wheel](https://packaging.python.org/en/latest/specifications/binary-distribution-format/):\n\n```bash\n$ poetry build\n```\n\nThis will generate `dist/not-again-ai-<version>.tar.gz` and `dist/not_again_ai-<version>-py3-none-any.whl`.\n\nRead more about the [advantages of wheels](https://pythonwheels.com/) to understand why generating\nwheel distributions are important.\n\n## Publish Distributions to PyPI\n\nSource and wheel redistributable packages can\nbe [published to PyPI](https://python-poetry.org/docs/cli#publish) or installed\ndirectly from the filesystem using `pip`.\n\n```bash\n$ poetry publish\n```\n\n# Enforcing Code Quality\n\nAutomated code quality checks are performed using \n[Nox](https://nox.thea.codes/en/stable/) and\n[`nox-poetry`](https://nox-poetry.readthedocs.io/en/stable/). Nox will automatically create virtual\nenvironments and run commands based on [`noxfile.py`](./noxfile.py) for unit testing, PEP 8 style\nguide checking, type checking and documentation generation.\n\n> Note: `nox` is installed into the virtual environment automatically by the `poetry install`\n> command above. Run `poetry shell` to activate the virtual environment.\n\nTo run all default sessions:\n\n```bash\n(.venv) $ nox\n```\n\n## Unit Testing\n\nUnit testing is performed with [pytest](https://pytest.org/). pytest has become the de facto Python\nunit testing framework. Some key advantages over the built-in\n[unittest](https://docs.python.org/3/library/unittest.html) module are:\n\n1. Significantly less boilerplate needed for tests.\n2. PEP 8 compliant names (e.g. `pytest.raises()` instead of `self.assertRaises()`).\n3. Vibrant ecosystem of plugins.\n\npytest will automatically discover and run tests by recursively searching for folders and `.py`\nfiles prefixed with `test` for any functions prefixed by `test`.\n\nThe `tests` folder is created as a Python package (i.e. there is an `__init__.py` file within it)\nbecause this helps `pytest` uniquely namespace the test files. Without this, two test files cannot\nbe named the same, even if they are in different subdirectories.\n\nCode coverage is provided by the [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/) plugin.\n\nWhen running a unit test Nox session (e.g. `nox -s test`), an HTML report is generated in\nthe `htmlcov` folder showing each source file and which lines were executed during unit testing.\nOpen `htmlcov/index.html` in a web browser to view the report. Code coverage reports help identify\nareas of the project that are currently not tested.\n\npytest and code coverage are configured in [`pyproject.toml`](./pyproject.toml).\n\nTo pass arguments to `pytest` through `nox`:\n\n```bash\n(.venv) $ nox -s test -- -k invalid_factorial\n```\n\n## Code Style Checking\n\n[PEP 8](https://peps.python.org/pep-0008/) is the universally accepted style guide for\nPython code. PEP 8 code compliance is verified using [Ruff](https://github.com/astral-sh/ruff).\nRuff is configured in the `[tool.ruff]` section of `pyproject.toml`.\n\nTo lint code, run:\n\n```bash\n(.venv) $ nox -s lint\n```\n\nTo automatically fix fixable lint errors, run:\n\n```bash\n(.venv) $ nox -s lint_fix\n```\n\n## Automated Code Formatting\n\nCode is automatically formatted using [black](https://github.com/psf/black). Imports are\nautomatically sorted and grouped using [Ruff](https://github.com/astral-sh/ruff).\n\nThese tools are configured by:\n\n- [`pyproject.toml`](./pyproject.toml)\n\nTo automatically format code, run:\n\n```bash\n(.venv) $ nox -s fmt\n```\n\nTo verify code has been formatted, such as in a CI job:\n\n```bash\n(.venv) $ nox -s fmt_check\n```\n\n## Type Checking\n\n[Type annotations](https://docs.python.org/3/library/typing.html) allows developers to include\noptional static typing information to Python source code. This allows static analyzers such\nas [mypy](http://mypy-lang.org/), [PyCharm](https://www.jetbrains.com/pycharm/),\nor [Pyright](https://github.com/microsoft/pyright) to check that functions are used with the\ncorrect types before runtime.\n\n\n```python\ndef factorial(n: int) -> int:\n    ...\n```\n\nmypy is configured in [`pyproject.toml`](./pyproject.toml). To type check code, run:\n\n```bash\n(.venv) $ nox -s type_check\n```\n\nSee also [awesome-python-typing](https://github.com/typeddjango/awesome-python-typing).\n\n### Distributing Type Annotations\n\n[PEP 561](https://www.python.org/dev/peps/pep-0561/) defines how a Python package should\ncommunicate the presence of inline type annotations to static type\ncheckers. [mypy\'s documentation](https://mypy.readthedocs.io/en/stable/installed_packages.html)\nprovides further examples on how to do this.\n\nMypy looks for the existence of a file named [`py.typed`](./src/not-again-ai/py.typed) in the root of the\ninstalled package to indicate that inline type annotations should be checked.\n\n## Continuous Integration\n\nContinuous integration is provided by [GitHub Actions](https://github.com/features/actions). This\nruns all tests, lints, and type checking for every commit and pull request to the repository.\n\nGitHub Actions is configured in [`.github/workflows/python.yml`](./.github/workflows/python.yml).\n\n## [Visual Studio Code](https://code.visualstudio.com/docs/languages/python)\n\nInstall the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VSCode.\n\nInstall the [Ruff extension](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff) for VSCode.\n\nDefault settings are configured in [`.vscode/settings.json`](./.vscode/settings.json). This will enable Ruff and black with consistent settings.\n\n# Documentation\n\n## Generating a User Guide\n\n[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) is a powerful static site\ngenerator that combines easy-to-write Markdown, with a number of Markdown extensions that increase\nthe power of Markdown. This makes it a great fit for user guides and other technical documentation.\n\nThe example MkDocs project included in this project is configured to allow the built documentation\nto be hosted at any URL or viewed offline from the file system.\n\nTo build the user guide, run,\n\n```bash\n(.venv) $ nox -s docs\n```\n\nand open `docs/user_guide/site/index.html` using a web browser.\n\nTo build the user guide, additionally validating external URLs, run:\n\n```bash\n(.venv) $ nox -s docs_check_urls\n```\n\nTo build the user guide in a format suitable for viewing directly from the file system, run:\n\n```bash\n(.venv) $ nox -s docs_offline\n```\n\nTo build and serve the user guide with automatic rebuilding as you change the contents,\nrun:\n\n```bash\n(.venv) $ nox -s docs_serve\n``` \n\nand open <http://127.0.0.1:8000> in a browser.\n\nEach time the `main` Git branch is updated, the \n[`.github/workflows/pages.yml`](.github/workflows/pages.yml) GitHub Action will\nautomatically build the user guide and publish it to [GitHub Pages](https://pages.github.com/).\nThis is configured in the `docs_github_pages` Nox session.\n\n## Generating API Documentation\n\nThis project uses [mkdocstrings](https://github.com/mkdocstrings/mkdocstrings) plugin for\nMkDocs, which renders\n[Google-style docstrings](https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html)\ninto an MkDocs project. Google-style docstrings provide a good mix of easy-to-read docstrings in\ncode as well as nicely-rendered output.\n\n```python\n"""Computes the factorial through a recursive algorithm.\n\nArgs:\n    n: A positive input value.\n\nRaises:\n    InvalidFactorialError: If n is less than 0.\n\nReturns:\n    Computed factorial.\n"""\n```\n\n## Misc\n\nIf you get a `Failed to create the collection: Prompt dismissed..` error when running `poetry update` on Ubuntu, try setting the following environment variable:\n\n    ```bash\n    export PYTHON_KEYRING_BACKEND=keyring.backends.null.Keyring\n    ```\n\n# Attributions\n[python-blueprint](https://github.com/johnthagen/python-blueprint) for the Python package skeleton.\n',
     'author': 'DaveCoDev',
     'author_email': 'dave.co.dev@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DaveCoDev/not-again-ai',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `not_again_ai-0.1.5/PKG-INFO` & `not_again_ai-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-again-ai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.
 Home-page: https://github.com/DaveCoDev/not-again-ai
 License: MIT
 Author: DaveCoDev
 Author-email: dave.co.dev@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -19,36 +19,38 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
-Requires-Dist: numpy (>=1.22.4,<2.0.0)
-Requires-Dist: pandas (>=1.4.2,<2.0.0)
-Requires-Dist: scikit-learn (>=1,<2)
-Requires-Dist: scipy (>=1,<2)
-Requires-Dist: seaborn (>=0,<1)
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Project-URL: Documentation, https://github.com/DaveCoDev/not-again-ai
 Project-URL: Repository, https://github.com/DaveCoDev/not-again-ai
 Description-Content-Type: text/markdown
 
 # not-again-ai
 
-[![GitHub Actions][github-actions-badge]](https://github.com/DaveCoDev/not-again-ai/actions)
+[![GitHub Actions][github-actions-badge]](https://github.com/johnthagen/python-blueprint/actions)
 [![Packaged with Poetry][poetry-badge]](https://python-poetry.org/)
-[![Code style: black][black-badge]](https://github.com/psf/black)
-[![Imports: isort][isort-badge]](https://pycqa.github.io/isort/)
+[![Nox][nox-badge]](https://github.com/wntrblm/nox)
+[![Code style: Black][black-badge]](https://github.com/psf/black)
+[![Ruff][ruff-badge]](https://github.com/astral-sh/ruff)
 [![Type checked with mypy][mypy-badge]](https://mypy-lang.org/)
 
-[github-actions-badge]: https://github.com/DaveCoDev/not-again-ai/workflows/python/badge.svg
+[github-actions-badge]: https://github.com/johnthagen/python-blueprint/workflows/python/badge.svg
+[poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg
+[nox-badge]: https://img.shields.io/badge/%F0%9F%A6%8A-Nox-D85E00.svg
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-[isort-badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+[ruff-badge]: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
 [mypy-badge]: https://www.mypy-lang.org/static/mypy_badge.svg
-[poetry-badge]: https://img.shields.io/badge/packaging-poetry-cyan.svg
 
 Have you ever been working on a project and groaned as you go to search again on how to nicely plot a simple distribution? Or have you been frustrated at wanting to run multiple functions in parallel, but stuck between the seemingly ten different ways to do it?
 **not-again-ai** is a Python package designed to once and for all collect all these little things that come up over and over again in AI projects and put them in one place.
 
 **Documentation** available at [DaveCoDev.github.io/not-again-ai/](https://DaveCoDev.github.io/not-again-ai/).
 
 # Installation
@@ -132,15 +134,15 @@
 
 # Development Information
 
 This package uses [Poetry](https://python-poetry.org/) to manage dependencies and
 isolated [Python virtual environments](https://docs.python.org/3/library/venv.html).
 
 To proceed, 
-[install Poetry globally onto your system](https://python-poetry.org/docs/#installation).
+[install Poetry globally onto your system](https://python-poetry.org/docs/#installing-with-the-official-installer).
 
 (Optional) configure Poetry to use an in-project virtual environment.
 ```bash
 $ poetry config virtualenvs.in-project true
 ```
 
 ## Dependencies
@@ -166,15 +168,15 @@
 
 To deactivate the environment:
 
 ```bash
 (.venv) $ exit
 ```
 
-To upgrade all dependencies to their latest versions:
+To upgrade all dependencies to the versions defined in [`pyproject.toml`](./pyproject.toml):
 
 ```bash
 $ poetry update
 ```
 
 ## Packaging
 
@@ -189,15 +191,15 @@
 [source distribution](https://packaging.python.org/en/latest/flow/#the-source-distribution-sdist) and
 a [wheel](https://packaging.python.org/en/latest/specifications/binary-distribution-format/):
 
 ```bash
 $ poetry build
 ```
 
-This will generate `dist/not-again-ai-0.1.0.tar.gz` and `dist/not_again_ai-0.1.0-py3-none-any.whl`.
+This will generate `dist/not-again-ai-<version>.tar.gz` and `dist/not_again_ai-<version>-py3-none-any.whl`.
 
 Read more about the [advantages of wheels](https://pythonwheels.com/) to understand why generating
 wheel distributions are important.
 
 ## Publish Distributions to PyPI
 
 Source and wheel redistributable packages can
@@ -256,37 +258,33 @@
 ```bash
 (.venv) $ nox -s test -- -k invalid_factorial
 ```
 
 ## Code Style Checking
 
 [PEP 8](https://peps.python.org/pep-0008/) is the universally accepted style guide for
-Python code. PEP 8 code compliance is verified using [Flake8](http://flake8.pycqa.org/). Flake8 is
-configured in the `[tool.flake8]` section of `pyproject.toml`. Extra Flake8 plugins are also
-included:
-
-- `flake8-bugbear`: Find likely bugs and design problems in your program.
-- `flake8-broken-line`: Forbid using backslashes (`\`) for line breaks.
-- `flake8-comprehensions`: Helps write better `list`/`set`/`dict` comprehensions.
-- `pep8-naming`: Ensure functions, classes, and variables are named with correct casing.
-- `flake8-pyproject`: Allow configuration of `flake8` through `pyproject.toml`.
-
-Some code style settings are included in [`.editorconfig`](./.editorconfig) and will be
-configured automatically in editors such as PyCharm.
+Python code. PEP 8 code compliance is verified using [Ruff](https://github.com/astral-sh/ruff).
+Ruff is configured in the `[tool.ruff]` section of `pyproject.toml`.
 
 To lint code, run:
 
 ```bash
 (.venv) $ nox -s lint
 ```
 
+To automatically fix fixable lint errors, run:
+
+```bash
+(.venv) $ nox -s lint_fix
+```
+
 ## Automated Code Formatting
 
 Code is automatically formatted using [black](https://github.com/psf/black). Imports are
-automatically sorted and grouped using [isort](https://github.com/PyCQA/isort/).
+automatically sorted and grouped using [Ruff](https://github.com/astral-sh/ruff).
 
 These tools are configured by:
 
 - [`pyproject.toml`](./pyproject.toml)
 
 To automatically format code, run:
 
@@ -339,15 +337,17 @@
 
 GitHub Actions is configured in [`.github/workflows/python.yml`](./.github/workflows/python.yml).
 
 ## [Visual Studio Code](https://code.visualstudio.com/docs/languages/python)
 
 Install the [Python extension](https://marketplace.visualstudio.com/items?itemName=ms-python.python) for VSCode.
 
-Default settings are configured in [`.vscode/settings.json`](./.vscode/settings.json). This will enable flake8 and black formatting with consistent settings.
+Install the [Ruff extension](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff) for VSCode.
+
+Default settings are configured in [`.vscode/settings.json`](./.vscode/settings.json). This will enable Ruff and black with consistent settings.
 
 # Documentation
 
 ## Generating a User Guide
 
 [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) is a powerful static site
 generator that combines easy-to-write Markdown, with a number of Markdown extensions that increase
```

