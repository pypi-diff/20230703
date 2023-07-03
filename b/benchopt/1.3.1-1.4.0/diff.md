# Comparing `tmp/benchopt-1.3.1.tar.gz` & `tmp/benchopt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/benchopt/benchopt/dist/.tmp-t24xaknm/benchopt-1.3.1.tar", last modified: Thu Dec  1 16:04:46 2022, max compression
+gzip compressed data, was "/home/runner/work/benchopt/benchopt/dist/.tmp-qo69fdgj/benchopt-1.4.0.tar", last modified: Mon Jul  3 07:17:57 2023, max compression
```

## Comparing `benchopt-1.3.1.tar` & `benchopt-1.4.0.tar`

### file list

```diff
@@ -1,182 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/.circleci/
--rw-r--r--   0 runner    (1001) docker     (116)       29 2022-12-01 16:04:33.000000 benchopt-1.3.1/.circleci/artifact_path
--rw-r--r--   0 runner    (1001) docker     (116)     5397 2022-12-01 16:04:33.000000 benchopt-1.3.1/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (116)      272 2022-12-01 16:04:33.000000 benchopt-1.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      853 2022-12-01 16:04:33.000000 benchopt-1.3.1/.github/workflows/expose_link.yml
--rw-r--r--   0 runner    (1001) docker     (116)      754 2022-12-01 16:04:33.000000 benchopt-1.3.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1894 2022-12-01 16:04:33.000000 benchopt-1.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     4282 2022-12-01 16:04:33.000000 benchopt-1.3.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)      476 2022-12-01 16:04:33.000000 benchopt-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1555 2022-12-01 16:04:33.000000 benchopt-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1240 2022-12-01 16:04:33.000000 benchopt-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      160 2022-12-01 16:04:33.000000 benchopt-1.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)    12515 2022-12-01 16:04:46.000000 benchopt-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     9992 2022-12-01 16:04:33.000000 benchopt-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/
--rw-r--r--   0 runner    (1001) docker     (116)      419 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18296 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    28126 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3788 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (116)    17664 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)    23059 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     5645 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/cli/process_results.py
--rw-r--r--   0 runner    (1001) docker     (116)     7050 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      226 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)       81 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4036 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/datasets/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     3004 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/datasets/tests/test_dataset_simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2743 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/helpers/julia.py
--rw-r--r--   0 runner    (1001) docker     (116)     1318 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/helpers/r_lang.py
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/helpers/requires_gpu.py
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/helpers/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/plotting/
--rw-r--r--   0 runner    (1001) docker     (116)     4020 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17546 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/generate_html.py
--rw-r--r--   0 runner    (1001) docker     (116)     1083 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2154 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/helpers_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/plotting/html/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/plotting/html/static/
--rw-r--r--   0 runner    (1001) docker     (116)      380 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/arrow_left.svg
--rw-r--r--   0 runner    (1001) docker     (116)     4947 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/benchmark.js
--rw-r--r--   0 runner    (1001) docker     (116)      686 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/download.svg
--rw-r--r--   0 runner    (1001) docker     (116)      841 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/home.svg
--rw-r--r--   0 runner    (1001) docker     (116)     6666 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/hover_index.css
--rw-r--r--   0 runner    (1001) docker     (116)     7664 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/main.css
--rw-r--r--   0 runner    (1001) docker     (116)    16816 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/result.js
--rw-r--r--   0 runner    (1001) docker     (116)    19163 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/symbols.js
--rw-r--r--   0 runner    (1001) docker     (116)    21919 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/static/utilities.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/plotting/html/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     6294 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/templates/benchmark.mako.html
--rw-r--r--   0 runner    (1001) docker     (116)     1977 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/templates/index.mako.html
--rw-r--r--   0 runner    (1001) docker     (116)    27423 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/html/templates/result.mako.html
--rw-r--r--   0 runner    (1001) docker     (116)     3856 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/plot_bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (116)     4994 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/plotting/plot_objective_curve.py
--rw-r--r--   0 runner    (1001) docker     (116)    11614 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/runner.py
--rw-r--r--   0 runner    (1001) docker     (116)    17375 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/stopping_criterion.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1142 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4760 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (116)     3537 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmark_features.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/
--rw-r--r--   0 runner    (1001) docker     (116)       51 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/
--rw-r--r--   0 runner    (1001) docker     (116)       89 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/
--rw-r--r--   0 runner    (1001) docker     (116)      124 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/dummy_subsubmodule/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/dummy_subsubmodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       31 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/func.py
--rw-r--r--   0 runner    (1001) docker     (116)       49 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/import_error.py
--rw-r--r--   0 runner    (1001) docker     (116)       44 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/value_error.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)     1336 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      715 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/leukemia.py
--rw-r--r--   0 runner    (1001) docker     (116)      972 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/simulated.py
--rw-r--r--   0 runner    (1001) docker     (116)       77 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/template_dataset.py
--rw-r--r--   0 runner    (1001) docker     (116)     1734 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/doc_objective.py
--rw-r--r--   0 runner    (1001) docker     (116)     1809 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/
--rw-r--r--   0 runner    (1001) docker     (116)     2482 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/cd.py
--rw-r--r--   0 runner    (1001) docker     (116)      381 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/julia_pgd.jl
--rw-r--r--   0 runner    (1001) docker     (116)      871 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/julia_pgd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1239 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd.py
--rw-r--r--   0 runner    (1001) docker     (116)     2242 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd_callback.py
--rw-r--r--   0 runner    (1001) docker     (116)      999 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.R
--rw-r--r--   0 runner    (1001) docker     (116)     1191 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.py
--rw-r--r--   0 runner    (1001) docker     (116)      786 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/solver_test.py
--rw-r--r--   0 runner    (1001) docker     (116)       77 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/template_solver.py
--rw-r--r--   0 runner    (1001) docker     (116)      608 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)      266 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/datasets/simulated.py
--rw-r--r--   0 runner    (1001) docker     (116)      627 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/solvers/
--rw-r--r--   0 runner    (1001) docker     (116)      317 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/solvers/baseline.py
--rw-r--r--   0 runner    (1001) docker     (116)     8271 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (116)    26896 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1492 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (116)     9926 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (116)     3824 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/test_stopping_criterion.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      204 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2164 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/utils/capture_run_output.py
--rw-r--r--   0 runner    (1001) docker     (116)     1648 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/tests/utils/patch_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      192 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      813 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/checkers.py
--rw-r--r--   0 runner    (1001) docker     (116)      971 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/class_property.py
--rw-r--r--   0 runner    (1001) docker     (116)     9400 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/conda_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (116)     6590 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/dependencies_mixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     3546 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/dynamic_modules.py
--rw-r--r--   0 runner    (1001) docker     (116)      804 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (116)     3690 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (116)     2445 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)     3836 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/parametrized_name_mixin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1327 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/pdb_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1160 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (116)     5078 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/safe_import.py
--rw-r--r--   0 runner    (1001) docker     (116)     4453 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/shell_cmd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1854 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/slurm_executor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2014 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/stream_redirection.py
--rw-r--r--   0 runner    (1001) docker     (116)     3757 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (116)     4821 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/terminal_output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2022-12-01 16:04:33.000000 benchopt-1.3.1/benchopt/utils/tests/test_conda_env_cmd.py
--rw-r--r--   0 runner    (1001) docker     (116)      176 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    12515 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5386 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       51 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      299 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-12-01 16:04:46.000000 benchopt-1.3.1/benchopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      310 2022-12-01 16:04:33.000000 benchopt-1.3.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (116)       39 2022-12-01 16:04:33.000000 benchopt-1.3.1/continuous_integration/build_doc.sh
--rw-r--r--   0 runner    (1001) docker     (116)      498 2022-12-01 16:04:33.000000 benchopt-1.3.1/continuous_integration/install_coverage_subprocess_pth.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1994 2022-12-01 16:04:33.000000 benchopt-1.3.1/continuous_integration/test_req_detection.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      666 2022-12-01 16:04:33.000000 benchopt-1.3.1/continuous_integration/test_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/doc/
--rw-r--r--   0 runner    (1001) docker     (116)     6058 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (116)   221083 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/_static/github_benchopt_token.png
--rw-r--r--   0 runner    (1001) docker     (116)     1471 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/doc/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/doc/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (116)      268 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (116)      271 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2529 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/_templates/search.html
--rw-r--r--   0 runner    (1001) docker     (116)     6090 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (116)      533 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1474 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6792 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     3479 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/config.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3912 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (116)    11456 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/how.rst
--rw-r--r--   0 runner    (1001) docker     (116)    12520 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      560 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/names.inc
--rw-r--r--   0 runner    (1001) docker     (116)     1899 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/publish.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/doc/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (116)      641 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2924 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/sphinxext/sphinx_click_semantic_group.py
--rw-r--r--   0 runner    (1001) docker     (116)     8017 2022-12-01 16:04:33.000000 benchopt-1.3.1/doc/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-01 16:04:46.000000 benchopt-1.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      105 2022-12-01 16:04:33.000000 benchopt-1.3.1/examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1224 2022-12-01 16:04:33.000000 benchopt-1.3.1/examples/plot_run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)     1144 2022-12-01 16:04:33.000000 benchopt-1.3.1/examples/plot_run_benchmark_python_R.py
--rw-r--r--   0 runner    (1001) docker     (116)      525 2022-12-01 16:04:33.000000 benchopt-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      599 2022-12-01 16:04:33.000000 benchopt-1.3.1/roadmap.md
--rw-r--r--   0 runner    (1001) docker     (116)     1588 2022-12-01 16:04:46.000000 benchopt-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      128 2022-12-01 16:04:33.000000 benchopt-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 07:17:45.000000 benchopt-1.4.0/.circleci/artifact_path
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-07-03 07:17:45.000000 benchopt-1.4.0/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-03 07:17:45.000000 benchopt-1.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 07:17:45.000000 benchopt-1.4.0/.github/workflows/expose_link.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-03 07:17:45.000000 benchopt-1.4.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-03 07:17:45.000000 benchopt-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-03 07:17:45.000000 benchopt-1.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 07:17:45.000000 benchopt-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-03 07:17:45.000000 benchopt-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 07:17:45.000000 benchopt-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 07:17:45.000000 benchopt-1.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-07-03 07:17:57.000000 benchopt-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-03 07:17:45.000000 benchopt-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28338 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22329 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/cli/process_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/datasets/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/datasets/tests/test_dataset_simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/helpers/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/helpers/r_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/helpers/requires_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/helpers/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/generate_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/helpers_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/plotting/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/plotting/html/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/arrow_left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/benchmark.js
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/hover_index.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/result.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19163 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/symbols.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/static/utilities.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/plotting/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/templates/benchmark.mako.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/templates/index.mako.html
+-rw-r--r--   0 runner    (1001) docker     (123)    30389 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/html/templates/result.mako.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/plot_bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/plotting/plot_objective_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11935 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/stopping_criterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmark_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/dummy_subsubmodule/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/dummy_subsubmodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/dummy_submodule/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/import_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/benchmark_utils/value_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/simulated.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/template_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/doc_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/julia_pgd.jl
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/julia_pgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.R
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/solver_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/template_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/datasets/simulated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/solvers/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31847 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/test_stopping_criterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/utils/capture_run_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/tests/utils/patch_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/class_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/conda_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/dependencies_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/dynamic_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/parametrized_name_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/pdb_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/safe_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/shell_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/slurm_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/stream_redirection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/terminal_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-03 07:17:45.000000 benchopt-1.4.0/benchopt/utils/tests/test_conda_env_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 07:17:57.000000 benchopt-1.4.0/benchopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-03 07:17:45.000000 benchopt-1.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-03 07:17:45.000000 benchopt-1.4.0/continuous_integration/build_doc.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-03 07:17:45.000000 benchopt-1.4.0/continuous_integration/install_coverage_subprocess_pth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1994 2023-07-03 07:17:45.000000 benchopt-1.4.0/continuous_integration/test_req_detection.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      666 2023-07-03 07:17:45.000000 benchopt-1.4.0/continuous_integration/test_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   221083 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/_static/github_benchopt_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/_templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/benchmark_list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/how.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/names.inc
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/performance_curves.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/publish.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/doc/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/sphinxext/sphinx_click_semantic_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/test_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-07-03 07:17:45.000000 benchopt-1.4.0/doc/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 07:17:57.000000 benchopt-1.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-03 07:17:45.000000 benchopt-1.4.0/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-03 07:17:45.000000 benchopt-1.4.0/examples/plot_run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-03 07:17:45.000000 benchopt-1.4.0/examples/plot_run_benchmark_python_R.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-03 07:17:45.000000 benchopt-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 07:17:45.000000 benchopt-1.4.0/roadmap.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-03 07:17:57.000000 benchopt-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-03 07:17:45.000000 benchopt-1.4.0/setup.py
```

### Comparing `benchopt-1.3.1/.circleci/config.yml` & `benchopt-1.4.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/.github/workflows/linting.yml` & `benchopt-1.4.0/.github/workflows/linting.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,31 @@
       - '**'
 
 jobs:
   check-manifest:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.9
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v3
       with:
         python-version: 3.9
 
     - name: Install dependencies
       run: pip install check-manifest
     - name: Check MANIFEST
       run: check-manifest
   flake8:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.9
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v3
       with:
         python-version: 3.9
 
     - name: Install dependencies
       run: pip install flake8
     - name: Flake8 linter
       run: flake8 .
```

### Comparing `benchopt-1.3.1/.github/workflows/release.yml` & `benchopt-1.4.0/.github/workflows/release.yml`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,17 @@
   create:
     tags:
       - '**'
 
 jobs:
   build-n-publish:
     name: Release to PyPI and TestPyPI 📦
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python 3.7
       uses: actions/setup-python@v1
       with:
         python-version: 3.7
     - name: Install pypa/build
```

### Comparing `benchopt-1.3.1/.github/workflows/test.yml` & `benchopt-1.4.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     defaults:
       run:
         # Need to use this shell to get cond working properly.
         # See https://github.com/marketplace/actions/setup-miniconda#important
         shell: bash -l {0}
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
           activate-environment: ${{ env.CONDA_ENV }}
           python-version: ${{ matrix.version_python }}
           # Use miniforge to only get conda-forge as default channel.
           miniforge-version: latest
```

### Comparing `benchopt-1.3.1/LICENSE` & `benchopt-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/MANIFEST.in` & `benchopt-1.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/PKG-INFO` & `benchopt-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchopt
-Version: 1.3.1
+Version: 1.4.0
 Summary: Benchmark toolkit for optimization
 Download-URL: https://github.com/benchopt/benchopt.git
 Maintainer: Thomas Moreau
 Maintainer-email: thomas.moreau@inria.fr
 License: BSD (3-clause)
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -22,115 +22,159 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: slurm
 License-File: LICENSE
 
-Benchmark repository for optimization
-=====================================
+.. image:: https://raw.githubusercontent.com/benchopt/communication_materials/main/posters/images/logo_benchopt.png
+   :width: 350
+   :align: center
+   
+*—Making your optimization benchmarks simple and open—*
+
+----
 
-|Test Status| |Python 3.6+| |codecov|
+|Test Status| |codecov| |Python 3.6+| |install-per-months| |discord| |SWH|
 
-BenchOpt is a benchmarking suite for optimization algorithms.
+``Benchopt`` is a benchmarking suite for optimization algorithms.
 It is built for simplicity, transparency, and reproducibility.
+It is implemented in Python but can run algorithms written in **many programming languages**.
 
-Benchopt is implemented in Python, and can run algorithms
-written in **many programming languages**
-(`example <https://benchopt.github.io/auto_examples/plot_run_benchmark_python_R.html>`_).
-So far, Benchopt has been tested with `Python <https://www.python.org/>`_,
+
+So far, ``benchopt`` has been tested with `Python <https://www.python.org/>`_,
 `R <https://www.r-project.org/>`_, `Julia <https://julialang.org/>`_
 and `C/C++ <https://isocpp.org/>`_ (compiled binaries with a command line interface).
-Programs available via
-`conda <https://docs.conda.io/en/latest/>`_ should be compatible.
+Programs available via `conda <https://docs.conda.io/en/latest/>`_ should be compatible as well.
+See for instance an `example of usage <https://benchopt.github.io/auto_examples/plot_run_benchmark_python_R.html>`_ with ``R``.
 
-BenchOpt is run through a command line interface as described
-in the `API Documentation <https://benchopt.github.io/api.html>`_.
-Replicating an optimization benchmark should
-be **as simple as doing**:
 
-.. code-block::
 
-   conda create -n benchopt python
-   conda activate benchopt
-   pip install benchopt
-   git clone https://github.com/benchopt/benchmark_logreg_l2
-   cd benchmark_logreg_l2
-   benchopt install -e . -s lightning -s sklearn
-   benchopt run -e . --config ./example_config.yml
+Install
+-------
 
-Running this command will give you a benchmark plot on l2-regularized
-logistic regression:
+It is recommended to use ``benchopt`` within a ``conda`` environment to fully-benefit
+from ``benchopt`` Command Line Interface (CLI).  
 
-.. figure:: https://benchopt.github.io/_images/sphx_glr_plot_run_benchmark_001.png
-   :target: how.html
-   :align: center
-   :scale: 80%
 
-See the `Available optimization problems`_ below.
+To install ``benchopt``, start by creating a new ``conda`` environment and then activate it
 
-Learn how to `create a new benchmark <https://benchopt.github.io/how.html>`_
-using the `benchmark template <https://github.com/benchopt/template_benchmark>`_.
+.. code-block::
 
-Install
---------
+    conda create -n benchopt python
+    conda activate benchopt
 
-The command line tool to run the benchmarks can be installed through `pip`. In order to allow `benchopt`
-to automatically install solvers dependencies, the install needs to be done in a `conda` environment.
 
+Then run the following command to install the **latest release** of ``benchopt``
 
 .. code-block::
 
-    conda create -n benchopt python
-    conda activate benchopt
+    pip install -U benchopt
 
-To get the **latest release**, use:
+
+It is also possible to use the **latest development version**. To do so, run instead
 
 .. code-block::
 
-    pip install benchopt
+    pip install -U -i https://test.pypi.org/simple/benchopt
 
-To get the **latest development version**, use:
 
-.. code-block::
 
-    pip install -U -i https://test.pypi.org/simple/ benchopt
+Getting started 
+---------------
 
-Then, existing benchmarks can be retrieved from git or created locally.
-For instance, the benchmark for Lasso can be retrieved with:
+After installing ``benchopt``, you can
 
-.. code-block::
+- replicate/modify an existing benchmark
+- create your own benchmark
 
-    git clone https://github.com/benchopt/benchmark_lasso
 
+Using an existing benchmark
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Command line interface
-----------------------
+Replicating an existing benchmark is simple.
+Here is how to do so for the `L2-logistic Regression benchmark <https://github.com/benchopt/benchmark_logreg_l2>`_.
 
-The preferred way to run the benchmarks is through the command line interface.
-To run the Lasso benchmark on all datasets and with all solvers, run:
+1. Clone the benchmark repository and ``cd`` to it
 
-.. code-block::
+.. code-block:: bash
 
-    benchopt run --env ./benchmark_lasso
+   git clone https://github.com/benchopt/benchmark_logreg_l2
+   cd benchmark_logreg_l2
 
-To get more details about the different options, run:
+2. Install the desired solvers automatically with ``benchopt``
 
-.. code-block::
+.. code-block:: bash
 
-    benchopt run -h
+   benchopt install . -s lightning -s sklearn
+
+3. Run the benchmark to get the figure below
+
+.. code-block:: bash
+
+   benchopt run . --config ./example_config.yml
+
+
+.. figure:: https://benchopt.github.io/_images/sphx_glr_plot_run_benchmark_001.png
+   :target: how.html
+   :align: center
+   :scale: 40%
 
-or read the `CLI documentation <https://benchopt.github.io/cli.html>`_.
 
-Benchopt also provides a Python API described in the
-`API documentation <https://benchopt.github.io/api.html>`_.
+These steps illustrate how to reproduce the `L2-logistic Regression benchmark <https://github.com/benchopt/benchmark_logreg_l2>`_.
+Find the complete list of the `Available benchmarks`_.
+Also, refer to the `documentation <https://benchopt.github.io/>`_ to learn more about ``benchopt`` CLI and its features.
+You can also easily extend this benchmark by adding a dataset, solver or metric.
+Learn that and more in the `Write a benchmark <https://benchopt.github.io/how.html>`_ tutorial.
 
 
-Available optimization problems
--------------------------------
+Creating a benchmark
+^^^^^^^^^^^^^^^^^^^^
+
+The section `Write a benchmark <https://benchopt.github.io/how.html>`_ of the documentation provides a tutorial
+for creating a benchmark. The ``benchopt`` community also maintains 
+a `template benchmark <https://github.com/benchopt/template_benchmark>`_ to quickly and easily start a new benchmark.
+
+
+
+Finding helps
+-------------
+
+Join ``benchopt`` `discord server <https://discord.gg/EA2HGQb7nv>`_ and get in touch with the community!
+Feel free to drop us a message to get help with running/constructing benchmarks 
+or (why not) discuss new features to be added and future development directions that ``benchopt`` should take.
+
+
+
+Citing Benchopt
+---------------
+
+``Benchopt`` is a continuous effort to make reproducible and transparent optimization benchmarks.
+Join us in this endeavor! If you use ``benchopt`` in a scientific publication, please cite
+
+.. code-block:: bibtex
+
+   @inproceedings{benchopt,
+      author    = {Moreau, Thomas and Massias, Mathurin and Gramfort, Alexandre 
+                   and Ablin, Pierre and Bannier, Pierre-Antoine 
+                   and Charlier, Benjamin and Dagréou, Mathieu and Dupré la Tour, Tom
+                   and Durif, Ghislain and F. Dantas, Cassio and Klopfenstein, Quentin
+                   and Larsson, Johan and Lai, En and Lefort, Tanguy 
+                   and Malézieux, Benoit and Moufad, Badr and T. Nguyen, Binh and Rakotomamonjy, 
+                   Alain and Ramzi, Zaccharie and Salmon, Joseph and Vaiter, Samuel},
+      title     = {Benchopt: Reproducible, efficient and collaborative optimization benchmarks},
+      year      = {2022},
+      booktitle = {NeurIPS},
+      url       = {https://arxiv.org/abs/2206.13424}
+   }
+
+
+
+Available benchmarks
+--------------------
 
 .. list-table::
    :widths: 70 15 15
    :header-rows: 1
 
    * - Problem
      - Results
@@ -144,77 +188,65 @@
    * - `LASSO: L1-Regularized Least Squares <https://github.com/benchopt/benchmark_lasso>`_
      - `Results <https://benchopt.github.io/results/benchmark_lasso.html>`__
      - |Build Status Lasso|
    * - `LASSO Path <https://github.com/jolars/benchmark_lasso_path>`_
      - `Results <https://benchopt.github.io/results/benchmark_lasso_path.html>`__
      - |Build Status Lasso Path|
    * - `Elastic Net <https://github.com/benchopt/benchmark_elastic_net>`_
-     - 
+     -
      - |Build Status ElasticNet|
    * - `MCP <https://github.com/benchopt/benchmark_mcp>`_
      - `Results <https://benchopt.github.io/results/benchmark_mcp.html>`__
      - |Build Status MCP|
    * - `L2-Regularized Logistic Regression <https://github.com/benchopt/benchmark_logreg_l2>`_
      - `Results <https://benchopt.github.io/results/benchmark_logreg_l2.html>`__
      - |Build Status LogRegL2|
    * - `L1-Regularized Logistic Regression <https://github.com/benchopt/benchmark_logreg_l1>`_
      - `Results <https://benchopt.github.io/results/benchmark_logreg_l1.html>`__
      - |Build Status LogRegL1|
    * - `L2-regularized Huber regression <https://github.com/benchopt/benchmark_huber_l2>`_
-     - 
+     -
      - |Build Status HuberL2|
    * - `L1-Regularized Quantile Regression <https://github.com/benchopt/benchmark_quantile_regression>`_
      - `Results <https://benchopt.github.io/results/benchmark_quantile_regression.html>`__
      - |Build Status QuantileRegL1|
    * - `Linear SVM for Binary Classification <https://github.com/benchopt/benchmark_linear_svm_binary_classif_no_intercept>`_
-     - 
+     -
      - |Build Status LinearSVM|
    * - `Linear ICA <https://github.com/benchopt/benchmark_linear_ica>`_
-     - 
+     -
      - |Build Status LinearICA|
    * - `Approximate Joint Diagonalization (AJD) <https://github.com/benchopt/benchmark_jointdiag>`_
-     - 
+     -
      - |Build Status JointDiag|
    * - `1D Total Variation Denoising <https://github.com/benchopt/benchmark_tv_1d>`_
      -
      - |Build Status TV1D|
    * - `2D Total Variation Denoising <https://github.com/benchopt/benchmark_tv_2d>`_
-     - 
+     -
      - |Build Status TV2D|
    * - `ResNet Classification <https://github.com/benchopt/benchmark_resnet_classif>`_
      - `Results <https://benchopt.github.io/results/benchmark_resnet_classif.html>`__
      - |Build Status ResNetClassif|
 
 
-Citing Benchopt
----------------
-
-If you use ``Benchopt`` in a scientific publication, please cite the following paper
-
-.. code-block:: bibtex
-
-   @article{benchopt,
-      author = {Moreau, Thomas and Massias, Mathurin and Gramfort, Alexandre and Ablin, Pierre 
-                and Bannier, Pierre-Antoine and Charlier, Benjamin and Dagréou, Mathieu and Dupré la Tour, Tom 
-                and Durif, Ghislain and F. Dantas, Cassio and Klopfenstein, Quentin 
-                and Larsson, Johan and Lai, En and Lefort, Tanguy and Malézieux, Benoit 
-                and Moufad, Badr and T. Nguyen, Binh and Rakotomamonjy, Alain and Ramzi, Zaccharie 
-                and Salmon, Joseph and Vaiter, Samuel},
-      title  = {Benchopt: Reproducible, efficient and collaborative optimization benchmarks},
-      year   = {2022},
-      url    = {https://arxiv.org/abs/2206.13424}
-   }
 
 
 .. |Test Status| image:: https://github.com/benchopt/benchopt/actions/workflows/test.yml/badge.svg
    :target: https://github.com/benchopt/benchopt/actions/workflows/test.yml
 .. |Python 3.6+| image:: https://img.shields.io/badge/python-3.6%2B-blue
    :target: https://www.python.org/downloads/release/python-360/
 .. |codecov| image:: https://codecov.io/gh/benchopt/benchopt/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/benchopt/benchopt
+.. |SWH| image:: https://archive.softwareheritage.org/badge/origin/https://github.com/benchopt/benchopt/
+    :target: https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/benchopt/benchopt
+.. |discord| image:: https://dcbadge.vercel.app/api/server/EA2HGQb7nv?style=flat
+   :target: https://discord.gg/EA2HGQb7nv
+.. |install-per-months| image:: https://static.pepy.tech/badge/benchopt/month
+   :target: https://pepy.tech/project/benchopt
 
 .. |Build Status OLS| image:: https://github.com/benchopt/benchmark_ols/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_ols/actions
 .. |Build Status NNLS| image:: https://github.com/benchopt/benchmark_nnls/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_nnls/actions
 .. |Build Status Lasso| image:: https://github.com/benchopt/benchmark_lasso/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_lasso/actions
```

### Comparing `benchopt-1.3.1/README.rst` & `benchopt-1.4.0/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,108 +1,152 @@
-Benchmark repository for optimization
-=====================================
+.. image:: https://raw.githubusercontent.com/benchopt/communication_materials/main/posters/images/logo_benchopt.png
+   :width: 350
+   :align: center
+   
+*—Making your optimization benchmarks simple and open—*
+
+----
 
-|Test Status| |Python 3.6+| |codecov|
+|Test Status| |codecov| |Python 3.6+| |install-per-months| |discord| |SWH|
 
-BenchOpt is a benchmarking suite for optimization algorithms.
+``Benchopt`` is a benchmarking suite for optimization algorithms.
 It is built for simplicity, transparency, and reproducibility.
+It is implemented in Python but can run algorithms written in **many programming languages**.
 
-Benchopt is implemented in Python, and can run algorithms
-written in **many programming languages**
-(`example <https://benchopt.github.io/auto_examples/plot_run_benchmark_python_R.html>`_).
-So far, Benchopt has been tested with `Python <https://www.python.org/>`_,
+
+So far, ``benchopt`` has been tested with `Python <https://www.python.org/>`_,
 `R <https://www.r-project.org/>`_, `Julia <https://julialang.org/>`_
 and `C/C++ <https://isocpp.org/>`_ (compiled binaries with a command line interface).
-Programs available via
-`conda <https://docs.conda.io/en/latest/>`_ should be compatible.
+Programs available via `conda <https://docs.conda.io/en/latest/>`_ should be compatible as well.
+See for instance an `example of usage <https://benchopt.github.io/auto_examples/plot_run_benchmark_python_R.html>`_ with ``R``.
 
-BenchOpt is run through a command line interface as described
-in the `API Documentation <https://benchopt.github.io/api.html>`_.
-Replicating an optimization benchmark should
-be **as simple as doing**:
 
-.. code-block::
 
-   conda create -n benchopt python
-   conda activate benchopt
-   pip install benchopt
-   git clone https://github.com/benchopt/benchmark_logreg_l2
-   cd benchmark_logreg_l2
-   benchopt install -e . -s lightning -s sklearn
-   benchopt run -e . --config ./example_config.yml
+Install
+-------
 
-Running this command will give you a benchmark plot on l2-regularized
-logistic regression:
+It is recommended to use ``benchopt`` within a ``conda`` environment to fully-benefit
+from ``benchopt`` Command Line Interface (CLI).  
 
-.. figure:: https://benchopt.github.io/_images/sphx_glr_plot_run_benchmark_001.png
-   :target: how.html
-   :align: center
-   :scale: 80%
 
-See the `Available optimization problems`_ below.
+To install ``benchopt``, start by creating a new ``conda`` environment and then activate it
 
-Learn how to `create a new benchmark <https://benchopt.github.io/how.html>`_
-using the `benchmark template <https://github.com/benchopt/template_benchmark>`_.
+.. code-block::
 
-Install
---------
+    conda create -n benchopt python
+    conda activate benchopt
 
-The command line tool to run the benchmarks can be installed through `pip`. In order to allow `benchopt`
-to automatically install solvers dependencies, the install needs to be done in a `conda` environment.
 
+Then run the following command to install the **latest release** of ``benchopt``
 
 .. code-block::
 
-    conda create -n benchopt python
-    conda activate benchopt
+    pip install -U benchopt
 
-To get the **latest release**, use:
+
+It is also possible to use the **latest development version**. To do so, run instead
 
 .. code-block::
 
-    pip install benchopt
+    pip install -U -i https://test.pypi.org/simple/benchopt
 
-To get the **latest development version**, use:
 
-.. code-block::
 
-    pip install -U -i https://test.pypi.org/simple/ benchopt
+Getting started 
+---------------
 
-Then, existing benchmarks can be retrieved from git or created locally.
-For instance, the benchmark for Lasso can be retrieved with:
+After installing ``benchopt``, you can
 
-.. code-block::
+- replicate/modify an existing benchmark
+- create your own benchmark
 
-    git clone https://github.com/benchopt/benchmark_lasso
 
+Using an existing benchmark
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Command line interface
-----------------------
+Replicating an existing benchmark is simple.
+Here is how to do so for the `L2-logistic Regression benchmark <https://github.com/benchopt/benchmark_logreg_l2>`_.
 
-The preferred way to run the benchmarks is through the command line interface.
-To run the Lasso benchmark on all datasets and with all solvers, run:
+1. Clone the benchmark repository and ``cd`` to it
 
-.. code-block::
+.. code-block:: bash
 
-    benchopt run --env ./benchmark_lasso
+   git clone https://github.com/benchopt/benchmark_logreg_l2
+   cd benchmark_logreg_l2
 
-To get more details about the different options, run:
+2. Install the desired solvers automatically with ``benchopt``
 
-.. code-block::
+.. code-block:: bash
 
-    benchopt run -h
+   benchopt install . -s lightning -s sklearn
+
+3. Run the benchmark to get the figure below
+
+.. code-block:: bash
+
+   benchopt run . --config ./example_config.yml
+
+
+.. figure:: https://benchopt.github.io/_images/sphx_glr_plot_run_benchmark_001.png
+   :target: how.html
+   :align: center
+   :scale: 40%
 
-or read the `CLI documentation <https://benchopt.github.io/cli.html>`_.
 
-Benchopt also provides a Python API described in the
-`API documentation <https://benchopt.github.io/api.html>`_.
+These steps illustrate how to reproduce the `L2-logistic Regression benchmark <https://github.com/benchopt/benchmark_logreg_l2>`_.
+Find the complete list of the `Available benchmarks`_.
+Also, refer to the `documentation <https://benchopt.github.io/>`_ to learn more about ``benchopt`` CLI and its features.
+You can also easily extend this benchmark by adding a dataset, solver or metric.
+Learn that and more in the `Write a benchmark <https://benchopt.github.io/how.html>`_ tutorial.
 
 
-Available optimization problems
--------------------------------
+Creating a benchmark
+^^^^^^^^^^^^^^^^^^^^
+
+The section `Write a benchmark <https://benchopt.github.io/how.html>`_ of the documentation provides a tutorial
+for creating a benchmark. The ``benchopt`` community also maintains 
+a `template benchmark <https://github.com/benchopt/template_benchmark>`_ to quickly and easily start a new benchmark.
+
+
+
+Finding helps
+-------------
+
+Join ``benchopt`` `discord server <https://discord.gg/EA2HGQb7nv>`_ and get in touch with the community!
+Feel free to drop us a message to get help with running/constructing benchmarks 
+or (why not) discuss new features to be added and future development directions that ``benchopt`` should take.
+
+
+
+Citing Benchopt
+---------------
+
+``Benchopt`` is a continuous effort to make reproducible and transparent optimization benchmarks.
+Join us in this endeavor! If you use ``benchopt`` in a scientific publication, please cite
+
+.. code-block:: bibtex
+
+   @inproceedings{benchopt,
+      author    = {Moreau, Thomas and Massias, Mathurin and Gramfort, Alexandre 
+                   and Ablin, Pierre and Bannier, Pierre-Antoine 
+                   and Charlier, Benjamin and Dagréou, Mathieu and Dupré la Tour, Tom
+                   and Durif, Ghislain and F. Dantas, Cassio and Klopfenstein, Quentin
+                   and Larsson, Johan and Lai, En and Lefort, Tanguy 
+                   and Malézieux, Benoit and Moufad, Badr and T. Nguyen, Binh and Rakotomamonjy, 
+                   Alain and Ramzi, Zaccharie and Salmon, Joseph and Vaiter, Samuel},
+      title     = {Benchopt: Reproducible, efficient and collaborative optimization benchmarks},
+      year      = {2022},
+      booktitle = {NeurIPS},
+      url       = {https://arxiv.org/abs/2206.13424}
+   }
+
+
+
+Available benchmarks
+--------------------
 
 .. list-table::
    :widths: 70 15 15
    :header-rows: 1
 
    * - Problem
      - Results
@@ -116,77 +160,65 @@
    * - `LASSO: L1-Regularized Least Squares <https://github.com/benchopt/benchmark_lasso>`_
      - `Results <https://benchopt.github.io/results/benchmark_lasso.html>`__
      - |Build Status Lasso|
    * - `LASSO Path <https://github.com/jolars/benchmark_lasso_path>`_
      - `Results <https://benchopt.github.io/results/benchmark_lasso_path.html>`__
      - |Build Status Lasso Path|
    * - `Elastic Net <https://github.com/benchopt/benchmark_elastic_net>`_
-     - 
+     -
      - |Build Status ElasticNet|
    * - `MCP <https://github.com/benchopt/benchmark_mcp>`_
      - `Results <https://benchopt.github.io/results/benchmark_mcp.html>`__
      - |Build Status MCP|
    * - `L2-Regularized Logistic Regression <https://github.com/benchopt/benchmark_logreg_l2>`_
      - `Results <https://benchopt.github.io/results/benchmark_logreg_l2.html>`__
      - |Build Status LogRegL2|
    * - `L1-Regularized Logistic Regression <https://github.com/benchopt/benchmark_logreg_l1>`_
      - `Results <https://benchopt.github.io/results/benchmark_logreg_l1.html>`__
      - |Build Status LogRegL1|
    * - `L2-regularized Huber regression <https://github.com/benchopt/benchmark_huber_l2>`_
-     - 
+     -
      - |Build Status HuberL2|
    * - `L1-Regularized Quantile Regression <https://github.com/benchopt/benchmark_quantile_regression>`_
      - `Results <https://benchopt.github.io/results/benchmark_quantile_regression.html>`__
      - |Build Status QuantileRegL1|
    * - `Linear SVM for Binary Classification <https://github.com/benchopt/benchmark_linear_svm_binary_classif_no_intercept>`_
-     - 
+     -
      - |Build Status LinearSVM|
    * - `Linear ICA <https://github.com/benchopt/benchmark_linear_ica>`_
-     - 
+     -
      - |Build Status LinearICA|
    * - `Approximate Joint Diagonalization (AJD) <https://github.com/benchopt/benchmark_jointdiag>`_
-     - 
+     -
      - |Build Status JointDiag|
    * - `1D Total Variation Denoising <https://github.com/benchopt/benchmark_tv_1d>`_
      -
      - |Build Status TV1D|
    * - `2D Total Variation Denoising <https://github.com/benchopt/benchmark_tv_2d>`_
-     - 
+     -
      - |Build Status TV2D|
    * - `ResNet Classification <https://github.com/benchopt/benchmark_resnet_classif>`_
      - `Results <https://benchopt.github.io/results/benchmark_resnet_classif.html>`__
      - |Build Status ResNetClassif|
 
 
-Citing Benchopt
----------------
-
-If you use ``Benchopt`` in a scientific publication, please cite the following paper
-
-.. code-block:: bibtex
-
-   @article{benchopt,
-      author = {Moreau, Thomas and Massias, Mathurin and Gramfort, Alexandre and Ablin, Pierre 
-                and Bannier, Pierre-Antoine and Charlier, Benjamin and Dagréou, Mathieu and Dupré la Tour, Tom 
-                and Durif, Ghislain and F. Dantas, Cassio and Klopfenstein, Quentin 
-                and Larsson, Johan and Lai, En and Lefort, Tanguy and Malézieux, Benoit 
-                and Moufad, Badr and T. Nguyen, Binh and Rakotomamonjy, Alain and Ramzi, Zaccharie 
-                and Salmon, Joseph and Vaiter, Samuel},
-      title  = {Benchopt: Reproducible, efficient and collaborative optimization benchmarks},
-      year   = {2022},
-      url    = {https://arxiv.org/abs/2206.13424}
-   }
 
 
 .. |Test Status| image:: https://github.com/benchopt/benchopt/actions/workflows/test.yml/badge.svg
    :target: https://github.com/benchopt/benchopt/actions/workflows/test.yml
 .. |Python 3.6+| image:: https://img.shields.io/badge/python-3.6%2B-blue
    :target: https://www.python.org/downloads/release/python-360/
 .. |codecov| image:: https://codecov.io/gh/benchopt/benchopt/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/benchopt/benchopt
+.. |SWH| image:: https://archive.softwareheritage.org/badge/origin/https://github.com/benchopt/benchopt/
+    :target: https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/benchopt/benchopt
+.. |discord| image:: https://dcbadge.vercel.app/api/server/EA2HGQb7nv?style=flat
+   :target: https://discord.gg/EA2HGQb7nv
+.. |install-per-months| image:: https://static.pepy.tech/badge/benchopt/month
+   :target: https://pepy.tech/project/benchopt
 
 .. |Build Status OLS| image:: https://github.com/benchopt/benchmark_ols/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_ols/actions
 .. |Build Status NNLS| image:: https://github.com/benchopt/benchmark_nnls/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_nnls/actions
 .. |Build Status Lasso| image:: https://github.com/benchopt/benchmark_lasso/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_lasso/actions
```

### Comparing `benchopt-1.3.1/benchopt/base.py` & `benchopt-1.4.0/benchopt/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tempfile
-import numbers
 import warnings
 
 from abc import ABC, abstractmethod
 
+from .callback import _Callback
+from .stopping_criterion import SingleRunCriterion
 from .stopping_criterion import SufficientProgressCriterion
 
 from .utils.safe_import import set_benchmark_module
 from .utils.dynamic_modules import get_file_hash
 from .utils.dynamic_modules import _reconstruct_class
 
 from .utils.dependencies_mixin import DependenciesMixin
@@ -65,15 +66,15 @@
             )
             return self.stop_strategy
         elif hasattr(self, 'stopping_strategy'):
             return self.stopping_strategy
         else:
             return self.stopping_criterion.strategy
 
-    def _set_objective(self, objective):
+    def _set_objective(self, objective, output=None):
         """Store the objective for hashing/pickling and check its compatibility
 
         Parameters
         ----------
         objective: benchopt.BaseObjective
             The objective function for the current optimization problem.
 
@@ -82,48 +83,61 @@
         skip : bool
             Whether this solver should be skipped or not for this objective.
         reason : str | None
             The reason why it should be skipped for display purposes.
             If skip is False, the reason should be None.
         """
         self._objective = objective
-        # XXX remove in version 1.4
+        self._output = output
+
         objective_dict = objective.get_objective()
-        if objective_dict is None:
-            assert hasattr(objective, "to_dict"), (
-                "Objective needs to implement `get_objective` that returns "
-                "a dictionary to be passed to `set_objective`"
-            )
-            warnings.warn(
-                "The method ``Objective.to_dict`` has been deprecated in "
-                "favor of ``Objective.get_objective``. Using it will no "
-                "longer work in version 1.4", FutureWarning
-            )
-            objective_dict = objective.to_dict()
+        assert objective_dict is not None, (
+            "Objective needs to implement `get_objective` that returns "
+            "a dictionary to be passed to `set_objective`"
+        )
 
         # Check if the objective is compatible with the solver
         skip, reason = self.skip(**objective_dict)
         if skip:
-            return skip, reason
+            self._output.skip(reason)
+            return True
 
         self.set_objective(**objective_dict)
-        return False, None
+        return False
 
     @abstractmethod
     def set_objective(self, **objective_dict):
         """Prepare the objective for the solver.
 
         Parameters
         ----------
         **objective_parameters : dict
             Dictionary obtained as the output of the method ``get_objective``
             from the benchmark ``Objective``.
         """
         ...
 
+    def pre_run_hook(self, stop_val):
+        """Hook to run pre-run operations.
+
+        This is mostly necessary to cache stop_val dependent computations, for
+        instance in ``jax`` with different number of iterations in a for loop.
+
+        Parameters
+        ----------
+        stop_val : int | float | callable
+            Value for the stopping criterion of the solver for. It allows to
+            sample the time/accuracy curve in the benchmark.
+            If it is a callable, then it should act as a callback. This
+            callback should be called once for each iteration with argument
+            the current iterate `parameters`. The callback returns False when
+            the computations should stop.
+        """
+        ...
+
     @abstractmethod
     def run(self, stop_val):
         """Call the solver with the given stop_val.
 
         This function should not return the parameters which will be
         retrieved by a subsequent call to get_result.
 
@@ -154,15 +168,15 @@
         -------
         parameters : ndarray, shape ``(dimension,)`` or ``*dimension``
             The computed coefficients by the solver.
         """
         ...
 
     def skip(self, **objective_dict):
-        """Used to decide if the ``Solver`` is compatible with the objective.
+        """Hook to decide if the ``Solver`` is compatible with the objective.
 
         Parameters
         ----------
         **objective_parameters : dict
             Dictionary obtained as the output of the method ``get_objective``
             from the benchmark ``Objective``.
 
@@ -179,32 +193,66 @@
 
         if not getattr(self, 'support_sparse', True):
             if any(sparse.issparse(v) for v in objective_dict.values()):
                 return True, f"{self} does not support sparse data."
 
         return False, None
 
+    def run_once(self, stop_val=1):
+        """Run the solver once, to cache warmup times (e.g. pre-compilations).
+
+        This function is intended to be called in ``Solver.set_objective``
+        method to avoid taking into account a solver's warmup costs.
+
+        Parameters
+        ----------
+        stop_val : int or float, (default: 1)
+            If ``stopping_strategy`` is 'iteration', this should be an integer
+            corresponding to the number of iterations the solver is run for.
+            If it is 'callback', it is an integer corresponding to the number
+            of times the callback is called.
+            If it is 'tolerance', it is a float which can be passed to call
+            the solver on an easy to solve problem.
+        """
+
+        if hasattr(self, '_output'):
+            self._output.progress('caching warmup times.')
+
+        if self._solver_strategy == "callback":
+            run_once_cb = _Callback(
+                lambda x: {'objective_value': 1},
+                {},
+                SingleRunCriterion(stop_val=stop_val).get_runner_instance(
+                    solver=self
+                )
+            )
+            run_once_cb.start()
+            self.run(run_once_cb)
+        else:
+            self.run(stop_val)
+
     @staticmethod
-    def _reconstruct(module_filename, parameters, objective,
+    def _reconstruct(module_filename, parameters, objective, output,
                      pickled_module_hash=None, benchmark_dir=None):
         set_benchmark_module(benchmark_dir)
         Solver = _reconstruct_class(
             module_filename, 'Solver', benchmark_dir, pickled_module_hash,
         )
         obj = Solver.get_instance(**parameters)
         if objective is not None:
-            obj._set_objective(objective)
+            obj._set_objective(objective, output=output)
         return obj
 
     def __reduce__(self):
         module_hash = get_file_hash(self._module_filename)
         objective = getattr(self, '_objective', None)
+        output = getattr(self, '_output', None)
         return self._reconstruct, (
-            self._module_filename, self._parameters, objective, module_hash,
-            str(self._import_ctx._benchmark_dir)
+            self._module_filename, self._parameters, objective, output,
+            module_hash, str(self._import_ctx._benchmark_dir)
         )
 
 
 class CommandLineSolver(BaseSolver, ABC):
     """A base class for solvers that are called through command lines
 
     The goal of this base class is to provide easy to use temporary files and
@@ -221,18 +269,17 @@
 
 
 class BaseDataset(ParametrizedNameMixin, DependenciesMixin, ABC):
     """Base class to define a dataset in a benchmark.
 
     Datasets that derive from this class should implement one method:
 
-    - ``get_data()``: retrieves/simulates the data contains in this data set
-      and returns the ``dimension`` of the data as well as a dictionary
-      containing the data. This dictionary is passed as arguments of the
-      objective function method ``set_data``.
+    - ``get_data()``: retrieves/simulates the data contained in this data set
+      and returns a dictionary containing the data. This dictionary is passed
+      as arguments of the objective's method ``set_data``.
     """
 
     _base_class_name = 'Dataset'
 
     @abstractmethod
     def get_data(self):
         """Return the data to feed to the objective .
@@ -248,32 +295,14 @@
     def _get_data(self):
         "Wrapper to make sure the returned results are correctly formated."
 
         # Automatically cache the _data to avoid reloading it.s
         if not hasattr(self, '_data') or self._data is None:
             self._data = self.get_data()
 
-            # XXX - Remove in version 1.3
-            if type(self._data) != dict:
-                import warnings
-                warnings.warn(
-                    "`get_data` should return a dict containing the data. "
-                    "The dimension should not be returned anymore and "
-                    "Objective should have a method `get_one_solution` "
-                    "to provide one feasible point. This will cause an "
-                    "error starting from version 1.3.",
-                    FutureWarning
-                )
-                dimension, data = self._data
-
-                # Make sure dimension is a tuple
-                if isinstance(dimension, numbers.Integral):
-                    dimension = (dimension,)
-                self._data = (dimension, data)
-
         return self._data
 
     # Reduce the pickling and hashing burden by only pickling class parameters.
     @staticmethod
     def _reconstruct(module_filename, pickled_module_hash, parameters,
                      benchmark_dir):
         set_benchmark_module(benchmark_dir)
@@ -324,16 +353,15 @@
         ----------
         **data: dict
             Extra parameters of the objective. This dictionary is retrieved
             by calling ``data = Dataset.get_data()``.
         """
         ...
 
-    # to uncomment in version 1.4, once `to_dict` has been deprecated.
-    # @abstractmethod
+    @abstractmethod
     def get_objective(self):
         """Return the objective parameters for the solver.
 
         Returns
         -------
         objective_dict: dict
             Parameters of the objective that will be given to the solver when
@@ -386,18 +414,14 @@
 
     # Save the dataset object used to get the objective data so we can avoid
     # hashing the data directly.
     def set_dataset(self, dataset):
         self._dataset = dataset
         data = dataset._get_data()
 
-        # XXX - Remove in version 1.3
-        if type(data) != dict:
-            self._dimension, data = data
-
         # Check if the dataset is compatible with the objective
         skip, reason = self.skip(**data)
         if skip:
             return skip, reason
 
         # Check if parameters are modified by set_data
         parameters = {}
@@ -435,44 +459,24 @@
             (accessible in the objective attributes).
         reason : str | None
             The reason why it should be skipped for display purposes.
             If skip is False, the reason should be None.
         """
         return False, None
 
+    @abstractmethod
     def get_one_solution(self):
         """Return one solution for which the objective can be evaluated.
 
-        This method is mainly for testing purposes, to check that the return
-        computation and the return type of `Objective.compute`. It should
-        return an object that can be passed to compute.
-
-        By default, if `Dataset.get_data` returns a shape, this function will
-        return an array full of 0. It can be overriden to provide a different
-        point. When `Dataset.get_data` returns "object", this method must be
-        overwritten.
-        """
-        if not hasattr(self, '_dimension'):
-            raise NotImplementedError(
-                "If solvers return objects, `Objective.get_one_solution` "
-                "should be overriden to return an object compatible with "
-                "`compute`."
-            )
-
-        # XXX - make this an abstract class in version 1.3
-        import warnings
-        warnings.warn(
-            "Objective should have a method `get_one_solution` "
-            "to provide one feasible point. This will cause an "
-            "error starting from version 1.3.",
-            FutureWarning
-        )
-
-        import numpy as np
-        return np.zeros(self._dimension)
+        This method is mainly for testing purposes, to check that the method
+        `Objective.compute` can be called and that it returns a compatible
+        type for benchopt. The returned object will be passed to
+        ``Objective.compute``.
+        """
+        pass
 
     # Reduce the pickling and hashing burden by only pickling class parameters.
     @staticmethod
     def _reconstruct(module_filename, pickled_module_hash, parameters,
                      dataset, benchmark_dir):
         set_benchmark_module(benchmark_dir)
         Objective = _reconstruct_class(
```

### Comparing `benchopt-1.3.1/benchopt/benchmark.py` & `benchopt-1.4.0/benchopt/benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,21 @@
                     "Could not find any Parquet nor "
                     f"CSV result files in {output_folder}."
                 )
             result_filename = all_result_files[-1]
             if filename == 'all':
                 result_filename = all_result_files
 
-        if result_filename.suffix == ".csv":
+        if isinstance(result_filename, list):
+            is_csv_file = any(fname.suffix == ".csv"
+                              for fname in result_filename)
+        else:
+            is_csv_file = result_filename.suffix == ".csv"
+
+        if is_csv_file:
             print(colorify(
                 "WARNING: CSV files are deprecated."
                 "Please use Parquet files instead.",
                 YELLOW
             ))
 
         return result_filename
```

### Comparing `benchopt-1.3.1/benchopt/callback.py` & `benchopt-1.4.0/benchopt/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,28 +52,30 @@
         # Initialize local variables
         self.info = get_sys_info()
         self.curve = []
         self.status = 'running'
         self.it = 0
         self.time_iter = 0.
         self.next_stopval = self.stopping_criterion.init_stop_val()
+
+    def start(self):
         self.time_callback = time.perf_counter()
 
     def __call__(self, x):
         # Stop time and update computation time since the beginning
         t0 = time.perf_counter()
 
         self.time_iter += t0 - self.time_callback
 
         # Evaluate the iteration if necessary.
         if self.it == self.next_stopval:
             if self.log_value(x):
                 return False
 
-        # Update iteration number and restart time measurment.
+        # Update iteration number and restart time measurement.
         self.it += 1
         self.time_callback = time.perf_counter()
         return True
 
     def log_value(self, x):
         """Store the objective value with running time and stop if needed.
```

### Comparing `benchopt-1.3.1/benchopt/cli/__init__.py` & `benchopt-1.4.0/benchopt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/cli/completion.py` & `benchopt-1.4.0/benchopt/cli/completion.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/cli/helpers.py` & `benchopt-1.4.0/benchopt/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/cli/main.py` & `benchopt-1.4.0/benchopt/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,39 +55,31 @@
         "slurm",
         "plot",
         "html",
         "pdb",
         "profile",
         "env_name",
         "output",
-        "objective_filter",
-        "old_objective_filter",
     ]
     return [cli_kwargs[name] for name in return_names]
 
 
 @main.command(
     help="Run a benchmark with benchopt.",
     epilog="To (re-)install the required solvers and datasets "
     "in a benchmark-dedicated conda environment or in your own "
     "conda environment, see the command `benchopt install`."
 )
 @click.argument('benchmark', default=Path.cwd(), type=click.Path(exists=True),
                 shell_complete=complete_benchmarks)
-@click.option('--objective-filter',
-              metavar='<objective_filter>', multiple=True, type=str,
-              help="Deprecated alias for `--objective`.")
 @click.option('--objective', '-o',
               metavar='<objective_filter>', multiple=True, type=str,
               help="Select the objective based on its parameters, with the "
               "syntax `objective[parameter=value]`. This can be used to only "
               "include one set of parameters. ")
-@click.option('--old-objective-filter', '-p',
-              multiple=True, type=str,
-              help="Deprecated alias for --objective_filter/-o.")
 @click.option('--solver', '-s',
               metavar="<solver_name>", multiple=True, type=str,
               help="Include <solver_name> in the benchmark. By default, all "
               "solvers are included. When `-s` is used, only listed solvers"
               " are included. Note that <solver_name> can include parameters,"
               " with the syntax `solver[parameter=value]`. "
               "To include multiple solvers, use multiple `-s` options.",
@@ -120,16 +112,18 @@
               help='Maximal number of runs for each solver. This corresponds '
               'to the number of points in the time/accuracy curve.')
 @click.option('--n-repetitions', '-r',
               metavar='<int>', default=1, show_default=True, type=int,
               help='Number of repetitions that are averaged to estimate the '
               'runtime.')
 @click.option('--timeout',
-              metavar="<int>", default=100, show_default=True, type=int,
-              help='Timeout a solver when run for more than <timeout> seconds')
+              default=100, show_default=True, type=str,
+              help='Stop a solver when run for more than <timeout> seconds.'
+              ' The syntax 10h or 10m can be used to denote 10 hours or '
+              'minutes respectively.')
 @click.option('--config', 'config_file', default=None,
               shell_complete=complete_config_files,
               help="YAML configuration file containing benchmark options.")
 @click.option('--plot/--no-plot', default=True,
               help="Whether or not to plot the results. Default is True.")
 @click.option('--html/--no-html', default=True,
               help="Whether to display the plot as HTML report or matplotlib"
@@ -171,35 +165,25 @@
 def run(config_file=None, **kwargs):
     if config_file is not None:
         with open(config_file, "r") as f:
             config = yaml.safe_load(f)
     else:
         config = {}
 
-    # XXX - Remove old and deprecated objective filters in version 1.3
     (
         benchmark, solver_names, forced_solvers, dataset_names,
         objective_filters, max_runs, n_repetitions, timeout, n_jobs, slurm,
-        plot, html, pdb, do_profile, env_name, output,
-        deprecated_objective_filters, old_objective_filters
+        plot, html, pdb, do_profile, env_name, output
     ) = _get_run_args(kwargs, config)
 
-    if len(old_objective_filters):
-        warnings.warn(
-            'Using the -p option is deprecated, use -o instead',
-            FutureWarning,
-        )
-        objective_filters = old_objective_filters
-
-    if len(deprecated_objective_filters):
-        warnings.warn(
-            'Using the --objective-filters option is deprecated, '
-            'use --objective instead', FutureWarning
-        )
-        objective_filters = deprecated_objective_filters
+    try:
+        timeout = int(float(timeout))
+    except ValueError:  # already under string format
+        import pandas as pd
+        timeout = pd.to_timedelta(timeout).total_seconds()
 
     # Create the Benchmark object
     benchmark = Benchmark(benchmark)
 
     if benchmark.min_version is not None:
         from packaging.version import parse
         from benchopt import __version__
@@ -467,16 +451,15 @@
         minimal=minimal, env_name=env_name, force=force, quiet=quiet,
     )
 
 
 @main.command(
     help="Test a benchmark for benchopt. The benchmark must feature a "
     "simulated dataset to test for all solvers. For more info about the "
-    "simulated dataset configurations, see"
-    "benchopt.github.io/how.html#example-of-parametrized-simulated-dataset",
+    "benchmark tests configuration and requirements, see :ref:`test_config`.",
     context_settings=dict(ignore_unknown_options=True)
 )
 @click.argument('benchmark', default=Path.cwd(), type=click.Path(exists=True),
                 shell_complete=complete_benchmarks)
 @click.option('--env-name', type=str, default=None, metavar='NAME',
               shell_complete=complete_conda_envs,
               help='Environment to run the test in. If it is not provided '
```

### Comparing `benchopt-1.3.1/benchopt/cli/process_results.py` & `benchopt-1.4.0/benchopt/cli/process_results.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/config.py` & `benchopt-1.4.0/benchopt/config.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/datasets/simulated.py` & `benchopt-1.4.0/benchopt/datasets/simulated.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/datasets/tests/test_dataset_simulated.py` & `benchopt-1.4.0/benchopt/datasets/tests/test_dataset_simulated.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/helpers/julia.py` & `benchopt-1.4.0/benchopt/helpers/julia.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/helpers/r_lang.py` & `benchopt-1.4.0/benchopt/helpers/r_lang.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/helpers/requires_gpu.py` & `benchopt-1.4.0/benchopt/helpers/requires_gpu.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/helpers/shell.py` & `benchopt-1.4.0/benchopt/helpers/shell.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/__init__.py` & `benchopt-1.4.0/benchopt/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/generate_html.py` & `benchopt-1.4.0/benchopt/plotting/generate_html.py`

 * *Files 13% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             datasets=datasets,
             sysinfo=sysinfo,
             dataset_names=df['data_name'].unique(),
             objective_names=df['objective_name'].unique(),
             obj_cols=[k for k in df.columns if k.startswith('objective_')
                       and k != 'objective_name'],
             kinds=list(kinds),
+            metadata=get_metadata(df),
         )
 
         # JSON
         result['json'] = json.dumps(shape_datasets_for_html(df))
 
         results.append(result)
 
@@ -119,14 +120,51 @@
             f"{benchmark_name}_"
             f"{html_file_name}"
         )
 
     return results
 
 
+def get_metadata(df):
+    """Get the benchmark metadata.
+
+    Metadata are already available among the columns of `df`.
+    It might be Objective and/or Solvers description.
+
+    Returns
+    -------
+    metadata: dict
+        Dictionary containing the benchmark metadata.
+    """
+    metadata = {}
+
+    # get solver descriptions
+    # wrap in try-except block to preserve compatibility
+    # with older versions
+    try:
+        solvers_description = df.groupby(
+            by=["solver_name"]
+        )["solver_description"].first()
+
+        metadata["solvers_description"] = solvers_description.to_dict()
+    except KeyError:
+        metadata["solvers_description"] = {}
+
+    # to avoid conflicts with objective metrics
+    # get objective description and use `obj_` instead of `objective_`
+    # try-except block to preserve compatibility with benchopt <= v1.3.1
+    try:
+        obj_description = df["obj_description"].unique()[0]
+        metadata["obj_description"] = obj_description
+    except KeyError:
+        metadata["obj_description"] = ""
+
+    return metadata
+
+
 def shape_datasets_for_html(df):
     """Return a dictionary with plotting data for each dataset."""
     datasets_data = {}
 
     for dataset in df['data_name'].unique():
         datasets_data[dataset] = shape_objectives_for_html(df, dataset)
 
@@ -175,31 +213,60 @@
     solver_data = {}
     for solver in df['solver_name'].unique():
         df_filtered = df.query("solver_name == @solver")
 
         # remove infinite values
         df_filtered = df_filtered.replace([np.inf, -np.inf], np.nan)
         df_filtered = df_filtered.dropna(subset=[objective_column])
+        if len(df_filtered) == 0:
+            continue
+
+        # compute median of 'time' and objective_column
+        fields = ["time", objective_column]
+        groupby_stop_val_median = df_filtered.groupby('stop_val')
+        groupby_stop_val_median = groupby_stop_val_median[fields]
+        groupby_stop_val_median = groupby_stop_val_median.median()
 
         q1, q9 = compute_quantiles(df_filtered)
+
         color, marker = get_solver_style(solver)
+        # to preserve support of previous benchopt version
+        # where 'stopping_strategy' wasn't saved in solver meta
+        try:
+            stopping_strategy = df_filtered['stopping_strategy'].unique()
+        except KeyError:
+            stopping_strategy = ["Time"]
+
+        if len(stopping_strategy) != 1:
+            found_stopping_strategies = ', '.join(
+                f"`{item}`" for item in stopping_strategy
+            )
+
+            raise Exception(
+                "Solver can be run using only one stopping strategy. "
+                f"Expected one stopping strategy "
+                f"but found {found_stopping_strategies}"
+            )
+
+        stopping_strategy = stopping_strategy[0]
+
         solver_data[solver] = {
             'scatter': {
-                'x': df_filtered.groupby('stop_val')['time']
-                                .median().tolist(),
-                'y': df_filtered.groupby('stop_val')[objective_column]
-                                .median().tolist(),
+                'x': groupby_stop_val_median['time'].tolist(),
+                'y': groupby_stop_val_median[objective_column].tolist(),
+                'stop_val': groupby_stop_val_median.index.tolist(),
                 'q1': q1.tolist(),
                 'q9': q9.tolist(),
             },
             'bar': {
                 **computeBarChartData(df, objective_column, solver)
             },
             'color': color,
-            'marker': marker
+            'marker': marker,
+            'stopping_strategy': stopping_strategy
         }
 
     return solver_data
 
 
 def get_sysinfo(df):
     """Get a dictionnary of the recorded system informations.
```

### Comparing `benchopt-1.3.1/benchopt/plotting/helpers.py` & `benchopt-1.4.0/benchopt/plotting/helpers.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/helpers_compat.py` & `benchopt-1.4.0/benchopt/plotting/helpers_compat.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/benchmark.js` & `benchopt-1.4.0/benchopt/plotting/html/static/benchmark.js`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/download.svg` & `benchopt-1.4.0/benchopt/plotting/html/static/download.svg`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/home.svg` & `benchopt-1.4.0/benchopt/plotting/html/static/home.svg`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/hover_index.css` & `benchopt-1.4.0/benchopt/plotting/html/static/hover_index.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,103 @@
 /*----------------------------------------*/
 /***** Stylesheet for the hover index *****/
 /*----------------------------------------*/
 
 /* Place rectangles in a grid */
 .grid {
-  position: relative; /* each rectangle is dependant of others */
+  position: relative;
+  /* each rectangle is dependant of others */
   margin: 0 auto;
-  padding: 1em 0 4em; /* padding top horizontal bottom */
-  display: grid; /* type of boxes generated */
+  padding: 1em 0 4em;
+  /* padding top horizontal bottom */
+  display: grid;
+  /* type of boxes generated */
   max-width: 1000px;
-  list-style: none; /* no item */
+  list-style: none;
+  /* no item */
   text-align: center;
-  column-gap: 2em; /* space between columns */
+  column-gap: 2em;
+  /* space between columns */
 }
 
 /* Figure inside grid */
 .grid figure {
   position: relative;
   float: left;
-  overflow: hidden; /* overflow not taken into account */
+  overflow: hidden;
+  /* overflow not taken into account */
   margin: 10px 1%;
-  width: 100%; /* 100% of the column */
+  width: 100%;
+  /* 100% of the column */
   background: #3085a3;
   text-align: center;
-  cursor: pointer; /* change shape cursor */
-  border-radius: 30px; /* rounded corners */
+  cursor: pointer;
+  /* change shape cursor */
+  border-radius: 30px;
+  /* rounded corners */
 }
 
 /* Each figure contains an img */
 .grid figure img {
   position: relative;
   display: block;
   max-height: 100%;
   max-width: 100%;
-  opacity: 1; /* over a dummy image */
+  opacity: 1;
+  /* over a dummy image */
 }
 
 /* Style caption (title of benchmarks) */
 .grid figure figcaption {
-  padding: 0.1em; /* add space */
-  color: #fff; /* writing color */
-  text-transform: uppercase; /* title in uppercase */
+  padding: 0.1em;
+  /* add space */
+  color: #fff;
+  /* writing color */
+  text-transform: uppercase;
+  /* title in uppercase */
   font-size: 1.25em;
 }
 
 /* Small sized screens */
 @media (min-width: 600px) {
   .grid {
     grid-template-columns: repeat(2, 1fr);
-  } /* split in 2 columns */
+  }
+
+  /* split in 2 columns */
 }
 
 /* Larger sized screens */
 @media (min-width: 900px) {
   .grid {
     grid-template-columns: repeat(3, 1fr);
-  } /* split in 3 columns */
+  }
+
+  /* split in 3 columns */
 }
 
 /* Position and style of <a> elements (the View more) */
 .grid figure figcaption,
-.grid figure figcaption > a {
+.grid figure figcaption>a {
   position: absolute;
-  top: 0em; /* no space offset top */
+  top: 0em;
+  /* no space offset top */
   left: 0;
   width: 100%;
   height: 100%;
 }
 
 /* only to figcaption <a> tag */
-.grid figure figcaption > a {
-  z-index: 1000; /* top level */
+.grid figure figcaption>a {
+  z-index: 1000;
+  /* top level */
   text-indent: 0%;
   white-space: nowrap;
-  font-size: 0; /* do not display the View more */
+  font-size: 0;
+  /* do not display the View more */
   opacity: 1;
 }
 
 /* h2: Problem name (LASSO, ...) */
 .grid figure h2 {
   word-spacing: 0em;
   font-weight: 300;
@@ -107,51 +127,61 @@
 figure.effect-ruby:hover {
   background-color: DodgerBlue;
 }
 
 /* Define transformation */
 figure.effect-ruby img {
   opacity: 0;
-  transition: opacity 0.35s, transform 0.35s; /* transition time */
-  transform: scale(1.15); /* size transformation -> bigger */
+  transition: opacity 0.35s, transform 0.35s;
+  /* transition time */
+  transform: scale(1.15);
+  /* size transformation -> bigger */
 }
 
 /* transformation with hovering */
 figure.effect-ruby:hover img {
   opacity: 0;
-  transform: scale(1); /* size -> smaller */
+  transform: scale(1);
+  /* size -> smaller */
 }
 
 /* Apply effect to problem name */
 figure.effect-ruby h2 {
   margin-top: 0;
-  transition: transform 0.35s; /* transition time */
+  transition: transform 0.35s;
+  /* transition time */
   transform: translate3d(0, calc((150px - 100%)/2), 0);
-  font-size: 1.25em; /* default font */
+  font-size: 1.25em;
+  /* default font */
 }
 
 figure.effect-ruby p {
   margin: 2em -1em 2em -1em;
   padding: 1em 0em 1em 0em;
-  border: 1px solid #fff; /* create sort of white frame */
+  border: 1px solid #fff;
+  /* create sort of white frame */
   opacity: 0;
   transition: opacity 0.35s, transform 0.35s;
-  transform: translate3d(0, 20px, 0) scale(1.1); /* size transform */
+  transform: translate3d(0, 20px, 0) scale(1.1);
+  /* size transform */
 }
 
 /* Transform title on hover */
 figure.effect-ruby:hover h2 {
   -webkit-transform: translate3d(0, 0, 0);
-  transform: translate3d(0px, 10px, 0) scale(0.8); /* smaller */
-  margin-top: 0em; /* move up */
+  transform: translate3d(0px, 10px, 0) scale(0.8);
+  /* smaller */
+  margin-top: 0em;
+  /* move up */
 }
 
 figure.effect-ruby:hover p {
   opacity: 1;
-  transform: translate3d(0, 0, 0) scale(1.2); /* placement in box */
+  transform: translate3d(0, 0, 0) scale(1.2);
+  /* placement in box */
 }
 
 /* Button for inside the table with system informations */
 .buttoncent {
   border: none;
   background-color: transparent;
   outline: none;
@@ -161,15 +191,16 @@
 /* button for inside text
  in benchmark page above graph for system informations */
 .buttonleft {
   border: none;
   background-color: transparent;
   outline: none;
   text-align: center;
-  margin-left: 1px; /* add margin */
+  margin-left: 1px;
+  /* add margin */
 }
 
 
 /* switch slider with an adaptable height.
 Change switch-height and switch-padding, and all the dimensions are adjusted.
 See https://stackoverflow.com/questions/70590125/how-to-change-the-size-of-a-css-toggle-switch */
 * {
@@ -258,16 +289,16 @@
   left: 0;
   height: 100%;
   width: 3px;
   background-color: #fff;
   transform-origin: 0 50%;
 }
 
-.ml11 .line1 { 
-  top: 0; 
+.ml11 .line1 {
+  top: 0;
   left: 0;
 }
 
 .ml11 .letter {
   display: inline-block;
   line-height: 1em;
   font-family: 'Kanit', sans-serif;
@@ -310,10 +341,102 @@
 }
 
 #legend_help {
   font-size: 0.75rem;
   color: #475569;
 }
 
-.space-r-2 > * {
+.space-r-2>* {
   margin-right: 0.5rem;
 }
+
+
+.objective-description-content {
+  visibility: hidden;
+
+  background-color: rgb(55 65 81);
+  color: #fff;
+  border-radius: 6px;
+  margin-top: 1.5em;
+  padding-right: 0.5em;
+  padding-left: 0.5em;
+  padding-top: 1em;
+  padding-bottom: 1em;
+  opacity: 90%;
+  max-width: 80ch;
+  max-height: 200px;
+
+  overflow-y: auto;
+  white-space: pre-wrap;
+  position: absolute;
+  z-index: 99999;
+}
+
+.objective-description-trigger {
+  display: flex;
+  flex-direction: row;
+}
+
+.objective-description-icon {
+  width: 1.25rem;
+  align-self: center;
+
+  border-radius: 50%;
+}
+
+.objective-description-trigger:hover .objective-description-content {
+  visibility: visible;
+}
+
+/* Description solver when hovered */
+.solver-description-container {
+  position: relative;
+  display: inline-flex;
+}
+
+.solver-description-content {
+  display: flex;
+  flex-direction: column;
+  visibility: hidden;
+  background-color: rgb(55 65 81);
+  color: #fff;
+  border-radius: 6px;
+  padding: 0.5em;
+  padding-right: 1rem;
+  opacity: 90%;
+
+  width: 400px;
+  max-height: 500px;
+  white-space: pre-wrap;
+
+  /* position description with respect to container and put it top-center */
+  position: absolute;
+  transform: translate(0, -100%);
+  z-index: 99999;
+}
+
+/* Show description when hovered */
+.solver-description-container:hover .solver-description-content {
+  visibility: visible;
+}
+
+/*Arrow at the bottom of the description*/
+.solver-description-container .solver-description-content::after {
+  content: " ";
+  position: absolute;
+  top: 100%;
+  left: 20px;
+  margin-left: -5px;
+  border-width: 7px;
+  border-style: solid;
+  border-color: rgb(55 65 81) transparent transparent transparent;
+}
+
+.solver-description-title {
+  margin-bottom: 1em;
+  font-weight: bolder;
+}
+
+.solver-description-body {
+  max-height: 450px;
+  overflow-y: auto;
+}
```

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/main.css` & `benchopt-1.4.0/benchopt/plotting/html/static/main.css`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/result.js` & `benchopt-1.4.0/benchopt/plotting/html/static/result.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -31,14 +31,21 @@
  */
 const setState = (partialState) => {
     window.state = {
         ...state(),
         ...partialState
     };
     displayScatterElements(!isBarChart());
+
+    // TODO: `listIdXaxisSelection` to be removed after 
+    // implementing responsiveness through breakpoints 
+    // and removing content duplication between big screen and mobile
+    let listIdXaxisSelection = ["change_xaxis_type", "change_xaxis_type_mobile"];
+    listIdXaxisSelection.forEach(idXaxisSelection => updateXaxis(idXaxisSelection))
+
     makePlot();
     makeLegend();
 }
 
 /**
  * Retrieve the state object from window.state
  *
@@ -127,61 +134,80 @@
  * @returns {array}
  */
 const getScatterCurves = () => {
     // create a list of object to plot in plotly
     const curves = [];
 
     // For each solver, add the median curve with proper style and visibility.
+    let xaxisType = state().xaxis_type;
+
     getSolvers().forEach(solver => {
+        solverStoppingStrategy = data(solver)['stopping_strategy'];
+
+        // plot only solvers that were stopped using xaxis type
+        // plot all solver if xaxis type is `time`
+        if (xaxisType !== "Time" && solverStoppingStrategy !== xaxisType) {
+            return
+        }
+
+        ScatterXaxisProperty = xaxisType === "Time" ? 'x' : 'stop_val';
+
         curves.push({
             type: 'scatter',
             name: solver,
             mode: 'lines+markers',
             line: {
                 color: data(solver).color,
             },
             marker: {
                 symbol: data(solver).marker,
                 size: 10,
             },
             legendgroup: solver,
             hovertemplate: solver + ' <br> (%{x:.1e},%{y:.1e}) <extra></extra>',
             visible: isVisible(solver) ? true : 'legendonly',
-            x: data(solver).scatter.x,
+            x: data(solver).scatter[ScatterXaxisProperty],
             y: useTransformer(data(solver).scatter.y, 'y', data().transformers),
         });
 
+        // skip plotting quantiles if xaxis is not time
+        // as stop_val are predefined and hence deterministic 
+        if (xaxisType !== "Time") {
+            return
+        }
+
         if (state().with_quantiles) {
             // Add shaded area for each solver, with proper style and visibility.
+
             curves.push({
                 type: 'scatter',
                 mode: 'lines',
                 showlegend: false,
                 line: {
                     width: 0,
                     color: data(solver).color,
                 },
                 legendgroup: solver,
                 hovertemplate: '(%{x:.1e},%{y:.1e}) <extra></extra>',
                 visible: isVisible(solver) ? true : 'legendonly',
-                x: data(solver).scatter.q1,
+                x: data(solver).scatter['q1'],
                 y: useTransformer(data(solver).scatter.y, 'y', data().transformers),
             }, {
                 type: 'scatter',
                 mode: 'lines',
                 showlegend: false,
                 fill: 'tonextx',
                 line: {
                     width: 0,
                     color: data(solver).color,
                 },
                 legendgroup: solver,
                 hovertemplate: '(%{x:.1e},%{y:.1e}) <extra></extra>',
                 visible: isVisible(solver) ? true : 'legendonly',
-                x: data(solver).scatter.q9,
+                x: data(solver).scatter['q9'],
                 y: useTransformer(data(solver).scatter.y, 'y', data().transformers),
             });
         }
     });
 
     return curves;
 };
@@ -357,14 +383,16 @@
             };
         default:
             console.error('Unknown scale value : ' + state().scale);
     }
 }
 
 const getScatterChartLayout = () => {
+    let xaxisType = state().xaxis_type;
+
     const layout = {
         autosize: !isSmallScreen(),
         modebar: {
             orientation: 'v',
         },
         height: 700,
         showlegend: false,
@@ -376,16 +404,16 @@
             xanchor: 'center',
             yanchor: 'top',
             y: -.2,
             x: .5
         },
         xaxis: {
             type: getScale().xaxis,
-            title: 'Time [sec]',
-            tickformat: '.1e',
+            title: xaxisType === "Time" ? "Time [sec]" : xaxisType,
+            tickformat: ["Time", "Tolerance"].includes(xaxisType) ? '.1e' : '',
             tickangle: -45,
             gridcolor: '#ffffff',
             zeroline: false,
         },
         yaxis: {
             type: getScale().yaxis,
             title: getYLabel(),
@@ -559,20 +587,36 @@
 /**
  * Creates the legend at the bottom of the plot.
  */
 const makeLegend = () => {
     const legend = document.getElementById('plot_legend');
 
     legend.innerHTML = '';
+    const solversDescription = window.metadata["solvers_description"];
 
     Object.keys(data().solvers).forEach(solver => {
         const color = data().solvers[solver].color;
         const symbolNumber = data().solvers[solver].marker;
 
-        legend.appendChild(createLegendItem(solver, color, symbolNumber));
+        let legendItem = createLegendItem(solver, color, symbolNumber);
+
+        // preserve compatibility with prev version
+        if (solversDescription === null || solversDescription === undefined) {
+            legend.appendChild(legendItem);
+            return;
+        }
+
+        let payload = {
+            title: solver,
+            description: solversDescription[solver],
+        }
+
+        legend.appendChild(
+            createSolverDescription(legendItem, payload)
+        );
     });
 }
 
 /**
  * Creates a legend item which contains the solver name,
  * the solver marker as an SVG and an horizontal bar with
  * the solver color.
@@ -646,14 +690,63 @@
     item.appendChild(createSymbol(symbolNumber, color));
     item.appendChild(hBar);
     item.appendChild(textContainer);
 
     return item;
 }
 
+
+function createSolverDescription(legendItem, {
+    title,
+    description
+}) {
+    if (description === null || description === undefined || description === "")
+        description = "No description provided";
+
+    let descriptionContainer = document.createElement("div");
+    descriptionContainer.setAttribute("class", "solver-description-container")
+
+    descriptionContainer.innerHTML = `
+  <div class="solver-description-content">
+    <span class="solver-description-title">${title}</span>
+    <span class="solver-description-body">${description}</span>
+  </div>
+  `;
+
+    descriptionContainer.prepend(legendItem);
+
+    return descriptionContainer;
+}
+
+
+function updateXaxis(idXaxisTypeSelection) {
+    let selection = document.getElementById(idXaxisTypeSelection);
+    selection.innerHTML = "";
+
+    let xaxisType = state()["xaxis_type"];
+    let options = new Set(['Time']);
+
+    // get solvers run for selected (dataset, objective, objective colum)
+    // and select their unique stopping strategies
+    let solvers = data()['solvers'];
+    Object.values(solvers).forEach(solver => options.add(solver['stopping_strategy']));
+
+    // create xaxis type options
+    options.forEach(option => {
+        element = document.createElement('option');
+        element.setAttribute('value', option);
+        element.innerText = option;
+
+        selection.append(element);
+    });
+
+    // set selected value
+    selection.value = options.has(xaxisType) ? xaxisType : "Time";
+}
+
 /**
  * Create the same svg symbol as plotly.
  * Returns an <svg> HTML Element
  *
  * @param {int} symbolNumber
  * @param {String} color
  * @returns {HTMLElement}
```

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/symbols.js` & `benchopt-1.4.0/benchopt/plotting/html/static/symbols.js`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/static/utilities.css` & `benchopt-1.4.0/benchopt/plotting/html/static/utilities.css`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/templates/benchmark.mako.html` & `benchopt-1.4.0/benchopt/plotting/html/templates/benchmark.mako.html`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/templates/index.mako.html` & `benchopt-1.4.0/benchopt/plotting/html/templates/index.mako.html`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/html/templates/result.mako.html` & `benchopt-1.4.0/benchopt/plotting/html/templates/result.mako.html`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,27 @@
                                     % for obj in result['objective_names']:
                                     <option value="${obj}">${obj}</option>
                                     %endfor
                                 </select>
                             </div>
                         </div>
                         <div class="mt-8 px-8">
-                            <label for="objective_column" class="block text-sm font-medium text-white">Objective column</label>
+                            <div class="flex flex-row items-center justify-between text-sm font-medium text-white">
+                                <label for="objective_column" class="block">Objective column</label>
+                                <!--don't show description unless it is provided -->
+                                % if result['metadata']['obj_description'] != "":
+                                    <span class="objective-description-trigger" style="cursor: pointer;">
+                                        <span style="margin-right: 0.5em;">description</span>
+                                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="objective-description-icon" viewBox="0 0 512 512">
+                                            <path d="M464 256A208 208 0 1 0 48 256a208 208 0 1 0 416 0zM0 256a256 256 0 1 1 512 0A256 256 0 1 1 0 256zm169.8-90.7c7.9-22.3 29.1-37.3 52.8-37.3h58.3c34.9 0 63.1 28.3 63.1 63.1c0 22.6-12.1 43.5-31.7 54.8L280 264.4c-.2 13-10.9 23.6-24 23.6c-13.3 0-24-10.7-24-24V250.5c0-8.6 4.6-16.5 12.1-20.8l44.3-25.4c4.7-2.7 7.6-7.7 7.6-13.1c0-8.4-6.8-15.1-15.1-15.1H222.6c-3.4 0-6.4 2.1-7.5 5.3l-.4 1.2c-4.4 12.5-18.2 19-30.6 14.6s-19-18.2-14.6-30.6l.4-1.2zM224 352a32 32 0 1 1 64 0 32 32 0 1 1 -64 0z"/>
+                                        </svg>
+                                        <div class="objective-description-content">${result['metadata']['obj_description']}</div>
+                                    </span>
+                                % endif
+                            </div>
                             <div class="mt-1 rounded-md shadow-sm">
                                 <select id="objective_column" class="focus:ring-blue-500 focus:border-blue-500 block w-full h-8 px-4 sm:text-sm border-gray-300 rounded-md" onchange="setState({objective_column: this.value})">
                                     % for obj_col in result['obj_cols']:
                                     <option value="${obj_col}">${obj_col}</option>
                                     %endfor
                                 </select>
                             </div>
@@ -81,14 +93,22 @@
                                     <option value="semilog-y">semilog-y</option>
                                     <option value="semilog-x">semilog-x</option>
                                     <option value="loglog">loglog</option>
                                     <option value="linear">linear</option>
                                 </select>
                             </div>
                         </div>
+                        <div id="xaxis-type-form-group" class="mt-8 px-8">
+                            <label for="change_scaling" class="block text-sm font-medium text-white">X-axis</label>
+                            <div class="mt-1 rounded-md shadow-sm">
+                                <select id="change_xaxis_type" class="focus:ring-blue-500 focus:border-blue-500 block w-full h-8 px-4 sm:text-sm border-gray-300 rounded-md" onchange="setState({xaxis_type: this.value})">
+                                   <!-- options will be added dynamically -->
+                                </select>
+                            </div>
+                        </div>
                         <div class="flex items-center justify-between mt-8 px-8">
                             <div class="block text-sm font-medium text-white">Quantiles</div>
                             <label class="block switch">
                                 <input id="change_shades" type="checkbox" checked onchange="setState({with_quantiles: this.checked})">
                                 <span class="slider round"></span>
                             </label>
                         </div>
@@ -213,14 +233,22 @@
                                         <option value="semilog-y">semilog-y</option>
                                         <option value="semilog-x">semilog-x</option>
                                         <option value="loglog">loglog</option>
                                         <option value="linear">linear</option>
                                     </select>
                                 </div>
                             </div>
+                            <div id="xaxis-type-form-group" class="mt-8 px-8">
+                                <label for="change_scaling" class="block text-sm font-medium text-white">X-axis</label>
+                                <div class="mt-1 rounded-md shadow-sm">
+                                    <select id="change_xaxis_type_mobile" class="focus:ring-blue-500 focus:border-blue-500 block w-full h-8 px-4 sm:text-sm border-gray-300 rounded-md" onchange="setState({xaxis_type: this.value})">
+                                       <!-- options will be added dynamically -->
+                                    </select>
+                                </div>
+                            </div>
                             <div class="flex items-center justify-between mt-8 px-8">
                                 <div class="block text-sm font-medium text-white">Quantiles</div>
                                 <label class="block switch">
                                     <input id="change_shades" type="checkbox" checked onchange="setState({with_quantiles: this.checked})">
                                     <span class="slider round"></span>
                                 </label>
                             </div>
@@ -365,24 +393,26 @@
                         translateX: [document.querySelector('.ml11 .letters').getBoundingClientRect().width + 10, document.querySelector('.ml11 .letters').getBoundingClientRect().width + 10],
                     });
             });
         </script>
         <!-- Manage plot -->
         <script>
             window.data = ${result['json']};
+            window.metadata = ${result['metadata']};
 
             window.addEventListener("load", () => {
                 // Initialize plot state
                 setState({
                     'dataset': document.getElementById('dataset_selector').value,
                     'objective': document.getElementById('objective_selector').value,
                     'objective_column': document.getElementById('objective_column').value,
                     'plot_kind': document.getElementById('plot_kind').value,
                     'scale': document.getElementById('change_scaling').value,
                     'with_quantiles': document.getElementById('change_shades').checked,
+                    'xaxis_type':  document.getElementById('change_xaxis_type').value || "Time",
                     'hidden_solvers': []
                 });
             });
         </script>
         <script type="text/javascript">
             ${static['symbols.js']}
             ${static['result.js']}
```

#### html2text {}

```diff
@@ -9,24 +9,28 @@
 % for data in result['dataset_names']:
 ${data}
 %endfor
 Objective:
 % for obj in result['objective_names']:
 ${obj}
 %endfor
-Objective column
+Objective column  % if result['metadata']['obj_description'] != "":
+description
+${result['metadata']['obj_description']}
+ % endif
 % for obj_col in result['obj_cols']:
 ${obj_col}
 %endfor
 Chart type
 % for kind in result['kinds']:
 ${kind}
 %endfor
 Scale
 [One of: semilog-y/semilog-x/loglog/linear]
+X-axis
 Quantiles
  *
 
   Benchopt    Open main menu
 Home Website Github
 Home Website Github Download_data
 
@@ -45,14 +49,15 @@
 %endfor
 Chart type
 % for kind in result['kinds']:
 ${kind}
 %endfor
 Scale
 [One of: semilog-y/semilog-x/loglog/linear]
+X-axis
 Quantiles
  *
 
 ***** Result on ${benchmark_name} benchmark *****
 % for name, val in result['sysinfo']['main'].items(): % if val != "":
 ${name.upper()} : ${val}
 % endif % endfor
```

### Comparing `benchopt-1.3.1/benchopt/plotting/plot_bar_chart.py` & `benchopt-1.4.0/benchopt/plotting/plot_bar_chart.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/plotting/plot_objective_curve.py` & `benchopt-1.4.0/benchopt/plotting/plot_objective_curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,21 +66,27 @@
         plt.text(0.5, 0.5, "Not Available")
         return fig
 
     for i, solver_name in enumerate(solver_names):
         df_ = df[df['solver_name'] == solver_name]
         curve = df_.groupby('stop_val').median(numeric_only=True)
 
-        q1 = df_.groupby('stop_val')['time'].quantile(.1)
-        q9 = df_.groupby('stop_val')['time'].quantile(.9)
+        # XXX: necessary since numpy 1.24.0 broke matplotolib compat
+        # with pandas. Remove once matplotlib/matplotlib#24773 is solved.
+        q1 = df_.groupby('stop_val')['time'].quantile(.1).to_numpy()
+        q9 = df_.groupby('stop_val')['time'].quantile(.9).to_numpy()
 
         color, marker = get_solver_style(solver_name, plotly=False)
         plt.loglog(curve['time'], curve[obj_col], color=color, marker=marker,
                    label=solver_name, linewidth=3)
-        plt.fill_betweenx(curve[obj_col], q1, q9, color=color, alpha=.3)
+
+        # XXX: ditto from above, remove to_numpy once compat is restored.
+        plt.fill_betweenx(
+            curve[obj_col].to_numpy(), q1, q9, color=color, alpha=.3
+        )
 
     if suboptimality and not relative:
         plt.hlines(eps, df['time'].min(), df['time'].max(), color='k',
                    linestyle='--')
         plt.xlim(df['time'].min(), df['time'].max())
 
     # Format the plot to be nice
@@ -141,14 +147,19 @@
 def compute_quantiles(df_filtered):
     q1 = df_filtered.groupby('stop_val')['time'].quantile(.1)
     q9 = df_filtered.groupby('stop_val')['time'].quantile(.9)
 
     return q1, q9
 
 
+def reset_solver_styles_idx():
+    "Reset solvers indices used to define colors and markers."
+    solvers_idx.clear()
+
+
 def get_solver_style(solver, plotly=True):
     idx = solvers_idx.get(solver, len(solvers_idx))
     solvers_idx[solver] = idx
 
     color = COLORS[idx % len(COLORS)]
     marker = MARKERS[idx % len(MARKERS)]
```

### Comparing `benchopt-1.3.1/benchopt/runner.py` & `benchopt-1.4.0/benchopt/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     """
     # check if the module caught a failed import
     if not solver.is_installed():
         raise ImportError(
             f"Failure during import in {solver.__module__}."
         )
 
+    solver.pre_run_hook(stop_val)
     t_start = time.perf_counter()
     solver.run(stop_val)
     delta_t = time.perf_counter() - t_start
     beta_hat_i = solver.get_result()
     objective_dict = objective(beta_hat_i)
 
     # Add system info in results
@@ -88,29 +89,22 @@
         The status on which the solver was stopped.
     """
 
     curve = []
     with exception_handler(output, pdb=pdb) as ctx:
 
         if solver._solver_strategy == "callback":
-            output.progress('empty run for compilation')
-            run_once_cb = _Callback(
-                lambda x: {'objective_value': 1},
-                {},
-                stopping_criterion.get_runner_instance(
-                    solver=solver, max_runs=1
-                )
-            )
-            solver.run(run_once_cb)
 
             # If stopping strategy is 'callback', only call once to get the
             # results up to convergence.
             callback = _Callback(
                 objective, meta, stopping_criterion
             )
+            solver.pre_run_hook(callback)
+            callback.start()
             solver.run(callback)
             curve, ctx.status = callback.get_results()
         else:
 
             # Create a Memory object to cache the computations in the benchmark
             # folder and handle cases where we force the run.
             run_one_resolution_cached = benchmark.cache(
@@ -176,30 +170,44 @@
 
     # Set objective an skip if necessary.
     skip, reason = objective.set_dataset(dataset)
     if skip:
         output.skip(reason, objective=True)
         return []
 
-    skip, reason = solver._set_objective(objective)
+    skip = solver._set_objective(objective, output=output)
     if skip:
-        output.skip(reason)
         return []
 
     states = []
     run_statistics = []
+
+    # get stopping strategy
+    # for plotting purpose consider 'callback' as 'iteration'
+    stopping_strategy = solver._solver_strategy
+    if stopping_strategy == 'callback':
+        stopping_strategy = 'iteration'
+
+    # get objective description
+    # use `obj_` instead of `objective_` to avoid conflicts with
+    # the name of metrics in Objective.compute
+    obj_description = objective.__doc__ or ""
+
     for rep in range(n_repetitions):
 
         output.set(rep=rep)
         # Get meta
         meta = dict(
             objective_name=str(objective),
             solver_name=str(solver),
             data_name=str(dataset),
             idx_rep=rep,
+            stopping_strategy=stopping_strategy.capitalize(),
+            obj_description=obj_description,
+            solver_description=solver.__doc__ or "",
         )
 
         stopping_criterion = solver.stopping_criterion.get_runner_instance(
             solver=solver,
             max_runs=max_runs,
             timeout=timeout / n_repetitions,
             output=output,
```

### Comparing `benchopt-1.3.1/benchopt/stopping_criterion.py` & `benchopt-1.4.0/benchopt/stopping_criterion.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,31 @@
 MAX_ITER = int(1e12)
 INFINITY = 3e38  # see: np.finfo('float32').max
 
 RHO = 1.5
 RHO_INC = 1.2  # multiplicative update if rho is too small
 
 
+COMMON_ARGS_DOC = """
+    strategy : str in {'iteration', 'tolerance', 'callback'}
+        How the different precision solvers are called. Can be one of:
+        - ``'iteration'``: call the run method with max_iter number increasing
+        logarithmically to get more an more precise points.
+        - ``'tolerance'``: call the run method with tolerance decreasing
+        logarithmically to get more and more precise points.
+        - ``'callback'``: call the run method with a callback that will compute
+        the objective function on a logarithmic scale. After each iteration,
+        the callback should be called with the current iterate solution.
+    key_to_monitor : str (default: 'objective_value')
+        The objective to check for tracking progress.
+"""
+
+
 class StoppingCriterion():
-    """Class to check if we need to stop an algorithm.
+    f"""Class to check if we need to stop an algorithm.
 
     This base class will check for the timeout and the max_run.
     It should be sub-classed to check for the convergence of the algorithm.
 
     This class also handles the detection of diverging solvers and prints the
     progress if given a ``progress_str``.
 
@@ -38,26 +53,15 @@
     plateau detection.
 
     Parameters
     ----------
     **kwargs : dict
         All parameters passed when instantiating the StoppingCriterion. This
         will be used to re-create the criterion with extra arguments in the
-        runner.
-    strategy : str in {'iteration', 'tolerance', 'callback'}
-        How the different precision solvers are called. Can be one of:
-        - ``'iteration'``: call the run method with max_iter number increasing
-        logarithmically to get more an more precise points.
-        - ``'tolerance'``: call the run method with tolerance decreasing
-        logarithmically to get more and more precise points.
-        - ``'callback'``: call the run method with a callback that will compute
-        the objective function on a logarithmic scale. After each iteration,
-        the callback should be called with the current iterate solution.
-    key_to_monitor : str (default: 'objective_value')
-        The objective to check for tracking progress.
+        runner.{COMMON_ARGS_DOC}
     """
     kwargs = None
 
     def __init__(self, strategy=None, key_to_monitor='objective_value',
                  **kwargs):
 
         assert strategy in STOPPING_STRATEGIES, (
@@ -123,25 +127,26 @@
         stopping_criterion.timeout = timeout
         stopping_criterion.max_runs = max_runs
         stopping_criterion.output = output
         stopping_criterion.solver = solver
 
         # Override get_next_stop_val if ``get_next`` is implemented for solver.
         if hasattr(solver, 'get_next'):
-            assert (
-                callable(solver.get_next)
-                # and type(solver.get_next) == staticmethod
-            ), "if defined, get_next should be a static method of the solver."
+            if not callable(solver.get_next):
+                raise TypeError(
+                    f"`get_next` of Solver in {solver.__module__} "
+                    "must be callable."
+                )
+
             try:
-                solver.get_next(0)
+                solver.get_next(1)
             except TypeError:
                 raise ValueError(
-                    "get_next(0) throw a TypeError. Verify that `get_next` "
-                    "signature is get_next(stop_val) and that it is "
-                    "a staticmethod."
+                    "get_next(1) throw a TypeError. Verify that `get_next` "
+                    "signature is get_next(self, stop_val)"
                 )
 
             stopping_criterion.get_next_stop_val = solver.get_next
 
         # Store running arguments
         if timeout is not None:
             stopping_criterion._deadline = time.time() + timeout
@@ -156,27 +161,27 @@
             INFINITY if self.strategy == 'tolerance' else 0
         )
 
         self.debug(f"Calling solver {self.solver} with stop val: {stop_val}")
         self.progress('initialization')
         return stop_val
 
-    def should_stop(self, stop_val, cost_curve):
+    def should_stop(self, stop_val, objective_list):
         """Base call to check if we should stop running a solver.
 
         This base call checks for the timeout and the max number of runs.
         It also notifies the runner if the curve is too flat, to increase
         the number of points between 2 evaluations of the objective.
 
         Parameters
         ----------
         stop_val : int | float
             Corresponds to stopping criterion of the underlying algorithm, such
             as ``tol`` or ``max_iter``.
-        cost_curve : list of dict
+        objective_list : list of dict
             List of dict containing the values associated to the objective at
             each evaluated points.
 
         Returns
         -------
         stop : bool
             Whether or not we should stop the algorithm.
@@ -186,18 +191,18 @@
             Next value for the stopping criterion. This value depends on the
             stop strategy for the solver.
         """
         # Modify the criterion state:
         # - compute the number of run with the curve. We need to remove 1 as
         #   it contains the initial evaluation.
         # - compute the delta_objective for debugging and stalled progress.
-        n_eval = len(cost_curve) - 1
-        objective = cost_curve[-1][self.key_to_monitor]
+        n_eval = len(objective_list) - 1
+        objective = objective_list[-1][self.key_to_monitor]
         delta_objective = self._prev_objective - objective
-        delta_objective /= abs(cost_curve[0][self.key_to_monitor])
+        delta_objective /= abs(objective_list[0][self.key_to_monitor])
         self._prev_objective = objective
 
         # default value for is_flat
         is_flat = False
 
         # check the different conditions:
         #     diverging / timeout / max_runs / stopping_criterion
@@ -210,15 +215,15 @@
 
         elif n_eval == self.max_runs:
             stop = True
             status = 'max_runs'
         else:
             # Call the sub-class hook, used to check stopping criterion
             # on the curve.
-            stop, progress = self.check_convergence(cost_curve)
+            stop, progress = self.check_convergence(objective_list)
 
             # Display the progress if necessary
             progress = max(n_eval / self.max_runs, progress)
 
             # Compute status and notify the runner if the curve is flat.
             status = 'done' if stop else 'running'
             is_flat = delta_objective == 0
@@ -236,20 +241,20 @@
         if status == 'running':
             stop_val = self.get_next_stop_val(stop_val)
             self.debug(f"Calling with stop val: {stop_val}")
             self.progress(progress=progress)
 
         return stop, status, stop_val
 
-    def check_convergence(self, cost_curve):
+    def check_convergence(self, objective_list):
         """Check if the solver should be stopped based on the objective curve.
 
         Parameters
         ----------
-        cost_curve : list of dict
+        objective_list : list of dict
             List of dict containing the values associated to the objective at
             each evaluated points.
 
         Returns
         -------
         stop : bool
             Whether or not we should stop the algorithm.
@@ -289,40 +294,28 @@
         if self.strategy == "tolerance":
             return min(1, max(stop_val / self.rho, MIN_TOL))
         else:
             return max(stop_val + 1, min(int(self.rho * stop_val), MAX_ITER))
 
 
 class SufficientDescentCriterion(StoppingCriterion):
-    """Stopping criterion based on sufficient descent.
+    f"""Stopping criterion based on sufficient descent.
 
     The solver will be stopped once successive evaluations do not make enough
     progress. The number of successive evaluation and the definition of
     sufficient progress is controlled by ``eps`` and ``patience``.
 
     Parameters
     ----------
     eps :  float (default: benchopt.stopping_criterion.EPS)
         The objective function change is considered as insufficient when it is
         in the interval ``[-eps, eps]``.
     patience :  float (default: benchopt.stopping_criterion.PATIENCE)
         The solver is stopped after ``patience`` successive insufficient
-        updates.
-    strategy : str in {'iteration', 'tolerance', 'callback'}
-        (default: 'iteration')
-        How the different precision solvers are called. Can be one of:
-        - ``'iteration'``: call the run method with max_iter number increasing
-        logarithmically to get more an more precise points.
-        - ``'tolerance'``: call the run method with tolerance decreasing
-        logarithmically to get more and more precise points.
-        - ``'callback'``: call the run method with a callback that will compute
-        the objective function on a logarithmic scale. After each iteration,
-        the callback should be called with the current iterate solution.
-    key_to_monitor : str (default: 'objective_value')
-        The objective to check for tracking progress.
+        updates.{COMMON_ARGS_DOC}
     """
 
     def __init__(self, eps=EPS, patience=PATIENCE, strategy='iteration',
                  key_to_monitor='objective_value'):
         self.eps = eps
         self.patience = patience
 
@@ -330,36 +323,36 @@
         self._objective = 1e100
 
         super().__init__(
             eps=eps, patience=patience, strategy=strategy,
             key_to_monitor=key_to_monitor
         )
 
-    def check_convergence(self, cost_curve):
+    def check_convergence(self, objective_list):
         """Check if the solver should be stopped based on the objective curve.
 
         Parameters
         ----------
-        cost_curve : list of dict
+        objective_list : list of dict
             List of dict containing the values associated to the objective at
             each evaluated points.
 
         Returns
         -------
         stop : bool
             Whether or not we should stop the algorithm.
         progress : float
             Measure of how far the solver is from convergence.
             This should be in [0, 1], 0 meaning no progress and 1 meaning
             that the solver has converged.
         """
         # Compute the current objective
-        objective = cost_curve[-1][self.key_to_monitor]
+        objective = objective_list[-1][self.key_to_monitor]
         delta_objective = self._objective - objective
-        delta_objective /= abs(cost_curve[0][self.key_to_monitor])
+        delta_objective /= abs(objective_list[0][self.key_to_monitor])
         self._objective = objective
 
         # Store only the last ``patience`` values for progress
         self._delta_objectives.append(delta_objective)
         if len(self._delta_objectives) > self.patience:
             self._delta_objectives.pop(0)
 
@@ -369,40 +362,28 @@
             return True, 1
 
         progress = math.log(max(abs(delta), self.eps)) / math.log(self.eps)
         return False, progress
 
 
 class SufficientProgressCriterion(StoppingCriterion):
-    """Stopping criterion based on sufficient progress.
+    f"""Stopping criterion based on sufficient progress.
 
     The solver will be stopped once successive evaluations do not make enough
     progress. The number of successive evaluation and the definition of
     sufficient progress is controlled by ``eps`` and ``patience``.
 
     Parameters
     ----------
     eps :  float (default: benchopt.stopping_criterion.EPS)
         The progress between two steps is considered as insufficient when it is
         smaller than ``eps``.
     patience :  float (default: benchopt.stopping_criterion.PATIENCE)
         The solver is stopped after ``patience`` successive insufficient
-        updates.
-    strategy : str in {'iteration', 'tolerance', 'callback'}
-        (default: 'iteration')
-        How the different precision solvers are called. Can be one of:
-        - ``'iteration'``: call the run method with max_iter number increasing
-        logarithmically to get more an more precise points.
-        - ``'tolerance'``: call the run method with tolerance decreasing
-        logarithmically to get more and more precise points.
-        - ``'callback'``: call the run method with a callback that will compute
-        the objective function on a logarithmic scale. After each iteration,
-        the callback should be called with the current iterate solution.
-    key_to_monitor : str (default: 'objective_value')
-        The objective to check for tracking progress.
+        updates.{COMMON_ARGS_DOC}
     """
 
     def __init__(self, eps=EPS, patience=PATIENCE, strategy='iteration',
                  key_to_monitor='objective_value'):
         self.eps = eps
         self.patience = patience
 
@@ -410,36 +391,36 @@
         self._best_objective = 1e100
 
         super().__init__(
             eps=eps, patience=patience, strategy=strategy,
             key_to_monitor=key_to_monitor
         )
 
-    def check_convergence(self, cost_curve):
+    def check_convergence(self, objective_list):
         """Check if the solver should be stopped based on the objective curve.
 
         Parameters
         ----------
-        cost_curve : list of dict
+        objective_list : list of dict
             List of dict containing the values associated to the objective at
             each evaluated points.
 
         Returns
         -------
         stop : bool
             Whether or not we should stop the algorithm.
         progress : float
             Measure of how far the solver is from convergence.
             This should be in [0, 1], 0 meaning no progress and 1 meaning
             that the solver has converged.
         """
         # Compute the current objective and update best value
-        objective = cost_curve[-1][self.key_to_monitor]
+        objective = objective_list[-1][self.key_to_monitor]
         delta_objective = self._best_objective - objective
-        delta_objective /= abs(cost_curve[0][self.key_to_monitor])
+        delta_objective /= abs(objective_list[0][self.key_to_monitor])
         self._best_objective = min(
             objective, self._best_objective
         )
 
         # Store only the last ``patience`` values for progress
         self._progress.append(delta_objective)
         if len(self._progress) > self.patience:
@@ -448,7 +429,48 @@
         delta = max(self._progress)
         if delta <= self.eps * self._best_objective:
             self.debug(f"Exit with delta = {delta:.2e}.")
             return True, 1
 
         progress = math.log(max(abs(delta), self.eps)) / math.log(self.eps)
         return False, progress
+
+
+class SingleRunCriterion(StoppingCriterion):
+    """Stopping criterion for single run solvers.
+
+    The solver will be stopped after one call to the objective.
+
+    Parameters
+    ----------
+    stop_val : int or float, (default: 1)
+        Value of ``stop_val`` with which the objective function will be called.
+        This value will be passed as ``n_iter`` or ``tol`` parameter for the
+        ``run`` method of solver with ``stopping_strategy`` respectively equals
+        to ``'iteration'`` or ``'tolerance'``, or the number of callback calls
+        minus one for the ``'callback'`` strategy.
+    """
+
+    def __init__(self, stop_val=1, *args, **kwargs):
+        # Necessary as the criterion is given a strategy argument when
+        # instanciated for an instance.
+        super().__init__(strategy="iteration", stop_val=stop_val)
+        self.stop_val = stop_val
+
+    def init_stop_val(self):
+        return self.stop_val
+
+    def get_runner_instance(self, max_runs=1, timeout=None, output=None,
+                            solver=None):
+
+        return super().get_runner_instance(1, timeout, output, solver)
+
+    def check_convergence(self, cost_curve):
+        return True, 1
+
+
+class NoCriterion(StoppingCriterion):
+    """Run the solvers for a number of time fixed by max_iter and timeout.
+    """
+
+    def check_convergence(self, cost_curve):
+        return False, 0
```

### Comparing `benchopt-1.3.1/benchopt/tests/__init__.py` & `benchopt-1.4.0/benchopt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/fixtures.py` & `benchopt-1.4.0/benchopt/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmark_features.py` & `benchopt-1.4.0/benchopt/tests/test_benchmark_features.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/dataset_test.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/dataset_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,33 +19,27 @@
     def __init__(
         self,
         n_samples=10,
         n_features=50,
         rho=0.6,
         random_state=27,
         skip=False,
-        deprecated_return=False
     ):
         # Store the parameters of the dataset
         self.n_samples = n_samples
         self.n_features = n_features
         self.random_state = random_state
         self.rho = rho
         self.skip = skip
-        self.deprecated_return = deprecated_return
 
     def get_data(self):
         rng = np.random.RandomState(self.random_state)
 
         X, y, _ = make_correlated_data(self.n_samples, self.n_features,
                                        rho=self.rho, random_state=rng)
         if self.skip:
             X = np.zeros_like(X)
             y = np.zeros_like(y)
 
         data = dict(X=X, y=y)
 
-        # XXX - Remove in version 1.3
-        if self.deprecated_return:
-            return self.n_features, data
-        else:
-            return data
+        return data
```

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/leukemia.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/leukemia.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/simulated.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/datasets/simulated.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/doc_objective.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/doc_objective.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/objective.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/objective.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,43 +2,44 @@
 
 
 with safe_import_context() as import_ctx:
     import numpy as np
 
 
 class Objective(BaseObjective):
+    """Here one can provide a description of the Objetive.
+
+    Lorem ipsum dolor sit amet. Eos voluptatem natus ab vero voluptatum est
+    excepturi saepe non minima alias sed laboriosam optio qui dolores autem
+    sit quae sequi. Cum dolorem maxime est perferendis dolores aut veritatis
+    officia ad voluptas quisquam in consequuntur aperiam qui optio sint.
+    """
+
     name = "Dummy Sparse Regression"
 
     # Make sure we can run with the current version
     min_benchopt_version = "0.0.0"
     parameters = {
         'reg': [0.05, .1, .5]
     }
 
-    def __init__(self, reg=.1, fit_intercept=False, deprecated_dataset=False):
+    def __init__(self, reg=.1, fit_intercept=False):
         self.reg = reg
         self.fit_intercept = fit_intercept
 
-        # XXX - Remove in version 1.3
-        self.deprecated_dataset = deprecated_dataset
-
     def set_data(self, X, y):
         self.X, self.y = X, y
         self.lmbd = self.reg * self._get_lambda_max()
 
     def skip(self, X, y):
         if np.all(X == 0):
             return True, 'X is all zeros'
         return False, None
 
     def get_one_solution(self):
-        # XXX - Remove in version 1.3
-        if self.deprecated_dataset:
-            return super().get_one_solution()
-
         return np.zeros(self.X.shape[1])
 
     def compute(self, beta):
         diff = self.y - self.X.dot(beta)
         objective_value = .5 * diff.dot(diff) + self.lmbd * abs(beta).sum()
 
         # To test for multiple type of return value, makes this depend on the
```

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/cd.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/cd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/julia_pgd.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/julia_pgd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd_callback.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/python_pgd_callback.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.R` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.R`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/r_pgd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/sklearn.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/sklearn.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/solver_test.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/solvers/solver_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,10 +48,9 @@
     def st(self, w, mu):
         w -= np.clip(w, -mu, mu)
         return w
 
     def get_result(self):
         return self.w
 
-    @staticmethod
-    def get_next(stop_val):
+    def get_next(self, stop_val):
         return stop_val + 1
```

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/dummy_benchmark/test_config.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/dummy_benchmark/test_config.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks/requirement_benchmark/objective.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks/requirement_benchmark/objective.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_benchmarks.py` & `benchopt-1.4.0/benchopt/tests/test_benchmarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import pytest
-import numbers
-import inspect
-
 import numpy as np
 
 from benchopt.runner import _Callback
 from benchopt.stopping_criterion import STOPPING_STRATEGIES
 from benchopt.utils import product_param
 
 
@@ -71,31 +68,14 @@
     if dataset_class.name.lower() == 'leukemia':
         pytest.skip("Leukemia download is broken in scikit-learn 1.1.0")
 
     data = dataset._get_data()
     assert isinstance(data, (tuple, dict)), (
         "Output of get_data should be a 2-tuple or a dict."
     )
-    # XXX - Remove in version 1.3
-    if isinstance(data, tuple):
-        assert len(data) == 2, (
-            "Output of get_data should be a 2-tuple"
-        )
-
-        dimension, data = data
-
-        assert isinstance(dimension, tuple) or dimension == 'object', (
-            "First output of get_data should be an integer or a tuple of "
-            f"integers. Got {dimension}."
-        )
-        if dimension != 'object':
-            assert all(isinstance(d, numbers.Integral) for d in dimension), (
-                "First output of get_data should be an integer or a tuple of "
-                f"integers. Got {dimension}."
-            )
 
     assert isinstance(data, dict), (
         f"The returned data from get_data should be a dict. Got {data}."
     )
 
 
 def test_solver_class(benchmark, solver_class):
@@ -110,34 +90,29 @@
     # Check that the solver_class uses a valid stopping_strategy
     if hasattr(solver_class, 'stopping_strategy'):
         msg = f"stopping_strategy should be in {STOPPING_STRATEGIES}."
         assert solver_class.stopping_strategy in STOPPING_STRATEGIES, msg
 
     # Check that the solver_class uses a valid callable to override get_next.
     if hasattr(solver_class, 'get_next'):
-        is_static = isinstance(
-            inspect.getattr_static(solver_class, "get_next"),
-            staticmethod
-        )
-        assert (callable(solver_class.get_next) and is_static), (
+        assert callable(solver_class.get_next), (
             "`get_next` for class Solver in "
-            f"'{solver_class.__module__}' should be a callable static method."
+            f"'{solver_class.__module__}' should be a callable."
         )
-        # Make sure the signature is def get_next(int):
-        solver_class.get_next(0)
+        # Make sure the signature is def get_next(self, int). Create instance
+        # of `solver_class` then call `get_next` since it is a class method
+        solver_class().get_next(0)
 
 
 def test_solver_install_api(benchmark, solver_class):
 
     # Check that the solver_class exposes a known install cmd
     assert solver_class.install_cmd in [None, 'conda', 'shell']
 
     # Check that the solver_class exposes a known install cmd
-    if solver_class.install_cmd == 'conda':
-        assert hasattr(solver_class, 'requirements')
     if solver_class.install_cmd == 'shell':
         assert hasattr(solver_class, 'install_script')
 
 
 @pytest.mark.requires_install
 def test_solver_install(test_env_name, benchmark, solver_class, check_test):
 
@@ -155,50 +130,54 @@
 
     # Check that a solver run with at least one configuration of a simulated
     # dataset.
 
     if not solver_class.is_installed():
         pytest.skip("Solver is not installed")
 
+    test_config = getattr(solver_class, "test_config", {})
+    objective_config = test_config.get('objective', {})
+    dataset_config = test_config.get('dataset', {})
+
     objective_class = benchmark.get_benchmark_objective()
-    objective = objective_class.get_instance()
+    objective = objective_class.get_instance(**objective_config)
 
     simulated_dataset = [
         d for d in benchmark.get_datasets() if d.name.lower() == 'simulated'
     ]
 
     assert len(simulated_dataset) == 1, (
         "All benchmark need to implement a simulated dataset for "
         "testing purpose. The dataset should have `name='simulated'."
     )
 
     dataset_class = simulated_dataset[0]
-    test_parameters = product_param(getattr(
-        dataset_class,
-        'test_parameters',
-        {},
+    dataset_test_parameters = product_param(getattr(
+        dataset_class, 'test_parameters', {}
     ))
-    if not test_parameters:
-        test_parameters = [{}]
+    if not dataset_test_parameters:
+        dataset_test_parameters = [{}]
     solver_ran_once = False
-    for test_params in test_parameters:
-        dataset = dataset_class.get_instance(**test_params)
+    for params in dataset_test_parameters:
+        params.update(dataset_config)
+        dataset = dataset_class.get_instance(**params)
 
         objective.set_dataset(dataset)
-
         solver = solver_class.get_instance()
-        skip, reason = solver._set_objective(objective)
+        skip = solver._set_objective(objective)
         if skip:
             continue
         solver_ran_once = True
         _test_solver_one_objective(solver, objective)
 
     assert solver_ran_once, (
-        'Solver skipped all simulated dataset configs. At least one simulated '
-        'dataset config should be compatible with a solver'
+        'Solver skipped all test configuration. At least one simulated '
+        'dataset and one objective config should be compatible with the '
+        'solver, potentially provided through "Solver.test_config" class '
+        'attribute or with `Dataset.test_parameters`.'
     )
 
 
 def _test_solver_one_objective(solver, objective):
     # Test a solver runs with a given objective and give proper result.
 
     is_convex = getattr(objective, "is_convex", True)
@@ -210,20 +189,21 @@
         )
         if not is_convex:
             # Set large tolerance for the stopping criterion to stop fast
             sc.eps = 5e-1
         cb = _Callback(
             objective, meta={}, stopping_criterion=sc
         )
+        cb.start()
         solver.run(cb)
     else:
         if solver._solver_strategy == 'iteration':
             stop_val = 5000 if is_convex else 2
         else:
-            stop_val = 1e-15 if is_convex else 1e-2
+            stop_val = 1e-10 if is_convex else 1e-2
         solver.run(stop_val)
 
     # Check that beta_hat is compatible to compute the objective function
     beta_hat = solver.get_result()
     objective(beta_hat)
 
     # Only check optimality or convex problems, with simple enough return type
```

### Comparing `benchopt-1.3.1/benchopt/tests/test_cli.py` & `benchopt-1.4.0/benchopt/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import re
 import time
 import tarfile
+import inspect
 import tempfile
 from pathlib import Path
 
 import click
 import pytest
 from joblib.memory import _FUNCTION_HASHES
 from click.shell_completion import ShellComplete
 
 from benchopt.benchmark import Benchmark
 from benchopt.plotting import PLOT_KINDS
 from benchopt.utils.stream_redirection import SuppressStd
+from benchopt.utils.dynamic_modules import _load_class_from_module
 
 
 from benchopt.tests import SELECT_ONE_PGD
 from benchopt.tests import SELECT_ONE_SIMULATED
 from benchopt.tests import SELECT_ONE_OBJECTIVE
 from benchopt.tests import TEST_BENCHMARK_DIR
 from benchopt.tests import DUMMY_BENCHMARK
@@ -142,14 +144,33 @@
         out.check_output('Dummy Sparse Regression', repetition=1)
         out.check_output(r'Python-PGD\[step_size=1\]:', repetition=6)
         out.check_output(r'Python-PGD\[step_size=1.5\]:', repetition=0)
 
         # Make sure the results were saved in a result file
         assert len(out.result_files) == 1, out.output
 
+    @pytest.mark.parametrize('timeout', ['10', '1m', '0.03h', '100s'])
+    def test_benchopt_run_in_env_timeout(self, test_env_name, timeout):
+        with CaptureRunOutput() as out:
+            with pytest.raises(SystemExit, match='False'):
+                run([str(DUMMY_BENCHMARK_PATH), '--env-name', test_env_name,
+                     '-d', SELECT_ONE_SIMULATED, '-f', SELECT_ONE_PGD,
+                     '-n', '1', '-r', '1', '-o', SELECT_ONE_OBJECTIVE,
+                     '--no-plot', '--timeout', timeout], 'benchopt',
+                    standalone_mode=False)
+
+        out.check_output(f'conda activate {test_env_name}')
+        out.check_output('Simulated', repetition=1)
+        out.check_output('Dummy Sparse Regression', repetition=1)
+        out.check_output(r'Python-PGD\[step_size=1\]:', repetition=6)
+        out.check_output(r'Python-PGD\[step_size=1.5\]:', repetition=0)
+
+        # Make sure the results were saved in a result file
+        assert len(out.result_files) == 1, out.output
+
     def test_benchopt_run_custom_parameters(self):
         SELECT_DATASETS = r'simulated[n_features=[100, 200]]'
         SELECT_SOLVERS = r'python-pgd-with-cb[use_acceleration=[True, False]]'
         SELECT_OBJECTIVES = r'dummy*[0.1, 0.2]'
 
         with CaptureRunOutput() as out:
             run([str(DUMMY_BENCHMARK_PATH), '-l', '-d', SELECT_DATASETS,
@@ -161,17 +182,17 @@
         out.check_output(r'Simulated\[n_features=200,', repetition=1)
         out.check_output(r'Simulated\[n_features=5000,', repetition=0)
         out.check_output(r'Dummy Sparse Regression\[reg=0.1\]', repetition=2)
         out.check_output(r'Dummy Sparse Regression\[reg=0.2\]', repetition=2)
         out.check_output(r'Dummy Sparse Regression\[reg=0.05\]', repetition=0)
         out.check_output(r'--Python-PGD\[', repetition=0)
         out.check_output(r'--Python-PGD-with-cb\[use_acceleration=False\]:',
-                         repetition=28)
+                         repetition=24)
         out.check_output(r'--Python-PGD-with-cb\[use_acceleration=True\]:',
-                         repetition=28)
+                         repetition=24)
 
     def test_benchopt_run_profile(self):
         with CaptureRunOutput() as out:
             run_cmd = [str(DUMMY_BENCHMARK_PATH),
                        '-d', SELECT_ONE_SIMULATED, '-f', SELECT_ONE_PGD,
                        '-n', '1', '-r', '1', '-o', SELECT_ONE_OBJECTIVE,
                        '--profile', '--no-plot']
@@ -190,15 +211,15 @@
         tmp.write("some_unknown_option: 0")
         tmp.flush()
         with pytest.raises(ValueError, match="Invalid config file option"):
             run(f'{str(DUMMY_BENCHMARK_PATH)} --config {tmp.name}'.split(),
                 'benchopt', standalone_mode=False)
 
         config = f"""
-        objective-filter:
+        objective:
           - {SELECT_ONE_OBJECTIVE}
         dataset:
           - {SELECT_ONE_SIMULATED}
         n-repetitions: 2
         max-runs: 1
         force-solver:
           - python-pgd[step_size=[2, 3]]
@@ -298,14 +319,80 @@
         )
 
         # Completion for datasets
         _test_shell_completion(
             run, [str(DUMMY_BENCHMARK_PATH), '-d'], DATASET_COMPLETION_CASES
         )
 
+    def test_import_ctx_name(self):
+        solver = inspect.cleandoc("""
+            from benchopt import BaseSolver, safe_import_context
+            with safe_import_context() as import_ctx_wrong_name:
+                import numpy as np
+
+
+            class Solver(BaseSolver):
+                name = "test_import_ctx"
+
+            """)
+        with tempfile.NamedTemporaryFile(
+                dir=DUMMY_BENCHMARK_PATH / "solvers",
+                mode='w', suffix='.py') as f:
+            f.write(solver)
+            f.flush()
+
+            err_msg = ("Import contexts should preferably be named import_ctx,"
+                       " got import_ctx_wrong_name.")
+            with pytest.warns(UserWarning, match=err_msg):
+                _load_class_from_module(
+                    f.name, "Solver",
+                    benchmark_dir=DUMMY_BENCHMARK_PATH
+                )
+
+    def test_handle_class_init_error(self):
+        # dataset with a wrong param name
+        dataset_src = (
+            "from benchopt import BaseDataset\n"
+            "class Dataset(BaseDataset):\n"
+            "    name = 'buggy-dataset'\n"
+            "    parameters = {'wrong_param_name': [1]}\n"
+            "    def __init__(self, param=1.):\n"
+            "        self.param = param\n"
+            "    def get_data(self):\n"
+            "        return dict()\n"
+        )
+        config = f"""
+            objective:
+            - {SELECT_ONE_OBJECTIVE}
+            dataset:
+            - buggy-dataset
+            max-runs: 1
+            solver:
+            - python-pgd[step_size=2]
+            """
+
+        TmpFileCtx = tempfile.NamedTemporaryFile
+        dataset_dir = DUMMY_BENCHMARK_PATH / "datasets"
+
+        with TmpFileCtx("w+", suffix='.py', dir=dataset_dir) as tmp_dataset, \
+             TmpFileCtx("w+") as tmp_config:
+
+            tmp_dataset.write(dataset_src)
+            tmp_dataset.flush()
+
+            tmp_config.write(config)
+            tmp_config.flush()
+
+            run_cmd = [str(DUMMY_BENCHMARK_PATH), '--config', tmp_config.name,
+                       '--no-plot']
+
+            error_match = """Dataset: "buggy-dataset".*'wrong_param_name'"""
+            with pytest.raises(TypeError, match=error_match):
+                run(run_cmd, 'benchopt', standalone_mode=False)
+
 
 class TestInstallCmd:
 
     @pytest.mark.parametrize('invalid_benchmark, match', [
         ('invalid_benchmark', "Path 'invalid_benchmark' does not exist."),
         ('.', "The folder '.' does not contain `objective.py`")],
         ids=['invalid_path', 'no_objective'])
@@ -375,14 +462,58 @@
             with pytest.raises(SystemExit, match='False'):
                 run_cmd = [str(REQUIREMENT_BENCHMARK_PATH), '--env-name',
                            test_env_name, '-n', '2', '-r', '1', '--no-plot']
                 run(run_cmd, 'benchopt', standalone_mode=False)
 
         out.check_output(r"done \(not enough run\)", repetition=1)
 
+    @pytest.mark.parametrize("cls_type", ['dataset', 'solver'])
+    def test_error_wih_missing_requirements(self, test_env_name, cls_type):
+        # if cls_type == "solver":
+        Cls = cls_type.capitalize()
+
+        # solver with missing dependency specified
+        src = (
+            f"from benchopt import Base{Cls}\n"
+            "from benchopt import safe_import_context\n"
+            "\n"
+            "with safe_import_context() as import_ctx:\n"
+            "    import sjdhfg\n"
+            f"class {Cls}(Base{Cls}):\n"
+            "    name = 'buggy-cls'\n"
+            "    def __init__(self):\n"
+            "        pass\n"
+            "    def set_objective(self):\n"
+            "        pass\n"
+            "    def get_data(self):\n"
+            "        {}\n"
+            "    def get_result(self):\n"
+            "        pass\n"
+            "    def run(self):\n"
+            "        pass\n"
+        )
+
+        TmpFileCtx = tempfile.NamedTemporaryFile
+        solver_dir = DUMMY_BENCHMARK_PATH / f"{cls_type}s"
+
+        with TmpFileCtx("w+", suffix='.py', dir=solver_dir) as tmp_solver:
+
+            tmp_solver.write(src)
+            tmp_solver.flush()
+
+            install_args = [
+                str(DUMMY_BENCHMARK_PATH),
+                '--env-name', test_env_name,
+                f'-{cls_type[0]}', "buggy-cls"
+            ]
+
+            error_match = f"Could not find dependencies for buggy-cls {Cls}"
+            with pytest.raises(AttributeError, match=error_match):
+                install(install_args, 'benchopt', standalone_mode=False)
+
     def test_shell_complete(self):
         # Completion for benchmark name
         _test_shell_completion(install, [], BENCHMARK_COMPLETION_CASES)
 
         # Completion for solvers
         _test_shell_completion(
             run, [str(DUMMY_BENCHMARK_PATH), '-s'], SOLVER_COMPLETION_CASES
```

### Comparing `benchopt-1.3.1/benchopt/tests/test_config.py` & `benchopt-1.4.0/benchopt/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/tests/test_runner.py` & `benchopt-1.4.0/benchopt/tests/test_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,32 +6,42 @@
 from benchopt.tests import TEST_DATASET
 from benchopt.tests import TEST_OBJECTIVE
 from benchopt.benchmark import _filter_classes
 from benchopt.benchmark import _extract_options
 from benchopt.benchmark import _extract_parameters
 
 
+class MockOutput:
+    def __init__(self):
+        self.reason = None
+
+    def skip(self, reason):
+        self.reason = reason
+
+
 def test_skip_api():
 
     dataset = TEST_DATASET.get_instance()
     objective = TEST_OBJECTIVE.get_instance(reg=0)
     objective.set_dataset(dataset)
 
     solver = TEST_SOLVER.get_instance()
 
-    skip, reason = solver._set_objective(objective)
+    out = MockOutput()
+    skip = solver._set_objective(objective, out)
     assert skip
-    assert reason == 'lmbd=0'
+    assert out.reason == 'lmbd=0'
 
     objective = TEST_OBJECTIVE.get_instance(reg=1)
     objective.set_dataset(dataset)
 
-    skip, reason = solver._set_objective(objective)
+    out = MockOutput()
+    skip = solver._set_objective(objective, out)
     assert not skip
-    assert reason is None
+    assert out.reason is None
 
     dataset = TEST_DATASET.get_instance(skip=True)
     objective = TEST_OBJECTIVE.get_instance()
     skip, reason = objective.set_dataset(dataset)
     assert skip
     assert reason == 'X is all zeros'
 
@@ -41,26 +51,14 @@
     objective = TEST_OBJECTIVE.get_instance()
     objective.set_dataset(dataset)
 
     one_solution = objective.get_one_solution()
     expected = np.zeros(objective.X.shape[1])
     assert all(one_solution == expected)
 
-    # XXX - Remove in version 1.3
-    dataset = TEST_DATASET.get_instance(deprecated_return=True)
-    objective = TEST_OBJECTIVE.get_instance(deprecated_dataset=True)
-
-    with pytest.warns(FutureWarning, match="`get_data` should return a dict"):
-        objective.set_dataset(dataset)
-
-    with pytest.warns(FutureWarning, match="Objective should have a method"):
-        one_solution = objective.get_one_solution()
-    expected = np.zeros(objective.X.shape[1])
-    assert all(one_solution == expected)
-
 
 def _assert_parameters_equal(instance, parameters):
     for key, val in parameters.items():
         assert getattr(instance, key) == val
 
 
 class TEST_DATASET_TWO_PARAMS(TEST_DATASET):
```

### Comparing `benchopt-1.3.1/benchopt/tests/test_stopping_criterion.py` & `benchopt-1.4.0/benchopt/tests/test_stopping_criterion.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,65 +12,65 @@
 ])
 def test_max_iter(criterion_class, strategy):
     "Check that max_runs stop correctly."
     criterion = criterion_class(strategy=strategy)
     criterion = criterion.get_runner_instance(max_runs=1)
 
     stop_val = criterion.init_stop_val()
-    cost_curve = [{'objective_value': 1}]
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list = [{'objective_value': 1}]
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert not stop, "Should not have stopped"
     assert status == 'running', "Should  be running"
 
-    cost_curve.append({'objective_value': .5})
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list.append({'objective_value': .5})
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert stop, "Should have stopped"
     assert status == 'max_runs', "Should stop on max_runs"
 
 
 @pytest.mark.parametrize('strategy', STOPPING_STRATEGIES)
 @pytest.mark.parametrize('criterion_class', [
     SufficientDescentCriterion, SufficientProgressCriterion
 ])
 def test_timeout(criterion_class, strategy):
     "Check that timeout=0 stopsimmediatly."
     criterion = criterion_class(strategy=strategy)
     criterion = criterion.get_runner_instance(timeout=0)
 
     stop_val = criterion.init_stop_val()
-    cost_curve = [{'objective_value': 1}]
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list = [{'objective_value': 1}]
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert stop, "Should have stopped"
     assert status == 'timeout', "Should stop on timeout"
 
 
 @pytest.mark.parametrize('strategy', STOPPING_STRATEGIES)
 @pytest.mark.parametrize('criterion_class', [
     SufficientDescentCriterion, SufficientProgressCriterion
 ])
 def test_diverged(criterion_class, strategy):
     "Check that the benchmark stops when diverging."
     criterion = criterion_class(strategy=strategy)
 
     criterion = criterion.get_runner_instance(max_runs=100)
     stop_val = criterion.init_stop_val()
-    cost_curve = [{'objective_value': 1}]
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list = [{'objective_value': 1}]
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert not stop, "Should not have stopped"
     assert status == 'running', "Should  be running"
 
-    cost_curve.append({'objective_value': 1e5+2})
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list.append({'objective_value': 1e5+2})
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert stop, "Should have stopped"
     assert status == 'diverged', "Should stop on diverged"
 
     criterion = criterion.get_runner_instance(max_runs=10)
     stop_val = criterion.init_stop_val()
-    cost_curve = [{'objective_value': np.nan}]
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list = [{'objective_value': np.nan}]
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert stop, "Should have stopped"
     assert status == 'diverged', "Should stop on diverged"
 
 
 @pytest.mark.parametrize('strategy', STOPPING_STRATEGIES)
 @pytest.mark.parametrize('criterion_class', [
     SufficientDescentCriterion, SufficientProgressCriterion
@@ -79,16 +79,16 @@
     "Check that the criterion tracks the right objective key."
     key = 'test'
     criterion = criterion_class(strategy=strategy, key_to_monitor=key)
 
     criterion = criterion.get_runner_instance(max_runs=10)
     assert criterion.key_to_monitor == key
     stop_val = criterion.init_stop_val()
-    cost_curve = [{'objective_value': np.nan, key: 1}]
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list = [{'objective_value': np.nan, key: 1}]
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert not stop, "Should not have stopped"
     assert status == 'running', "Should stop on diverged"
 
-    cost_curve.append({key: 1e5+2})
-    stop, status, stop_val = criterion.should_stop(stop_val, cost_curve)
+    objective_list.append({key: 1e5+2})
+    stop, status, stop_val = criterion.should_stop(stop_val, objective_list)
     assert stop, "Should have stopped"
     assert status == 'diverged', "Should stop on diverged"
```

### Comparing `benchopt-1.3.1/benchopt/tests/utils/capture_run_output.py` & `benchopt-1.4.0/benchopt/tests/utils/capture_run_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,10 +55,10 @@
         matches = re.findall(pattern, output)
         if repetition is None:
             assert len(matches) > 0, (
                 f"Could not find '{pattern}' in output:\n{output}"
             )
         else:
             assert len(matches) == repetition, (
-                f"Could not find {repetition} x '{pattern}' in output:\n"
-                f"{output}"
+                f"Found {len(matches)} repetitions instead of {repetition} of"
+                f"'{pattern}' in output:\n{output}"
             )
```

### Comparing `benchopt-1.3.1/benchopt/tests/utils/patch_benchmark.py` & `benchopt-1.4.0/benchopt/tests/utils/patch_benchmark.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/checkers.py` & `benchopt-1.4.0/benchopt/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/class_property.py` & `benchopt-1.4.0/benchopt/utils/class_property.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/conda_env_cmd.py` & `benchopt-1.4.0/benchopt/utils/conda_env_cmd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/dynamic_modules.py` & `benchopt-1.4.0/benchopt/utils/dynamic_modules.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities to load classes and module from filenames and class names.
 """
 import sys
 import hashlib
+import warnings
 import importlib
 from pathlib import Path
 
 from .safe_import import safe_import_context
 
 
 def _get_module_from_file(module_filename, benchmark_dir=None):
@@ -58,17 +59,29 @@
     benchmark_dir = Path(benchmark_dir)
     module_filename = Path(module_filename)
     module = _get_module_from_file(module_filename, benchmark_dir)
     klass = getattr(module, class_name)
 
     # Store the info to easily reload the class
     klass._module_filename = module_filename.resolve()
-    klass._import_ctx = getattr(
-            module, 'import_ctx', safe_import_context()
-    )
+
+    klass._import_ctx = getattr(module, 'import_ctx', None)
+    if klass._import_ctx is None:
+        for var_name in dir(module):
+            var = getattr(module, var_name)
+            if isinstance(var, safe_import_context):
+                klass._import_ctx = var
+                warnings.warn(
+                    "Import contexts should preferably be named import_ctx, "
+                    f"got {var_name}.",  UserWarning
+                )
+                break
+        else:
+            klass._import_ctx = safe_import_context()
+
     klass._benchmark_dir = benchmark_dir.resolve()
     return klass
 
 
 def get_file_hash(filename):
     """Compute the MD5 hash of a file.
     """
```

### Comparing `benchopt-1.3.1/benchopt/utils/files.py` & `benchopt-1.4.0/benchopt/utils/files.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/github.py` & `benchopt-1.4.0/benchopt/utils/github.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/misc.py` & `benchopt-1.4.0/benchopt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/parametrized_name_mixin.py` & `benchopt-1.4.0/benchopt/utils/parametrized_name_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,17 +34,28 @@
 
         Saving the parameters allow for cheap hashing and to compute parametric
         names for the objects.
         """
         try:
             obj = cls(**parameters)
             obj.save_parameters(**parameters)
-        except Exception:
-            print(cls)
+        except Exception as exception:
+            # get type (Dataset, Objective, or Solver) of class and its name
+            cls_type = cls.__base__.__name__
+            cls_type = cls_type.replace("Base", "")
+            cls_name = cls.name
+
+            # Extend exception error message
+            # TODO: use `add_note` when requiring python>=3.11
+            exception.args = (
+                f'Error when initializing {cls_type}: "{cls_name}". '
+                f'{". ".join(exception.args)}',
+            )
             raise
+
         return obj
 
     @property
     @abstractmethod
     def name(self):
         """Each object should expose its name for plotting purposes."""
         ...
```

### Comparing `benchopt-1.3.1/benchopt/utils/pdb_helpers.py` & `benchopt-1.4.0/benchopt/utils/pdb_helpers.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/profiling.py` & `benchopt-1.4.0/benchopt/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/safe_import.py` & `benchopt-1.4.0/benchopt/utils/safe_import.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,19 +46,14 @@
     that a solver/dataset is not installed.
 
     Moreover, this context also allows to skip the import when simply listing
     all solvers, for benchmark's installation or auto completion. Note that all
     costly imports should be protected with this import for benchopt to perform
     best.
 
-    This context is also used to import module dynamically from the ``utils``
-    folder of a benchmark, using the
-    :func:`~benchopt.safe_import_context.import_from` method.
-    See :ref:`benchmark_utils_import` for a detailed explanation of this part.
-
     Finally, this context also catches import warnings.
     """
 
     def __init__(self):
         self.failed_import = False
         self.record = warnings.catch_warnings(record=True)
         self._benchmark_dir = BENCHMARK_DIR
@@ -76,61 +71,14 @@
         if not RAISE_INSTALL_ERROR:
             self.record.__enter__()
         return self
 
     def trace(self, frame, event, arg):
         raise SkipWithBlock()
 
-    def import_from(self, module_name, obj=None):
-        """Dynamically import a module from BENCHMARK_DIR/utils.
-
-        Parameters
-        ----------
-        module_name: str
-            Name of the module to import. It can be a module with a simple
-            ``*.py`` file, or a more complex package with a ``__init__.py``
-            file. The naming convention for import is the same, with submodules
-            separated with ``.``. The module is imported directly from the
-            BENCHMARK_DIR/utils/ folder.
-        obj: str or None
-            If ``obj`` is provided, the module is imported and only the
-            attribute named ``obj`` from this module is returned.
-
-        Returns
-        -------
-        module or obj: object
-            Module or object imported dynamically.
-        """
-
-        # XXX: To remove in benchopt 1.4
-        warnings.warn(
-            "import_from is deprecated. Please import reusable code for the "
-            "benchmark from `benchmark_utils` module in the root dir of the "
-            "benchmark folder.", FutureWarning
-        )
-
-        module_path = BENCHMARK_DIR / 'utils' / module_name.replace('.', '/')
-        if not module_path.exists():
-            module_path = module_path.with_suffix('.py')
-        elif module_path.is_dir():
-            module_path = module_path / '__init__.py'
-        if not module_path.exists():
-            raise ValueError(
-                f"Failed to import {module_name}. Check that file "
-                f" {module_path} exists in the benchmark."
-            )
-
-        # import locally to avoid circular import
-        from .dynamic_modules import _get_module_from_file
-        module = _get_module_from_file(module_path, BENCHMARK_DIR)
-        if obj is None:
-            return module
-        else:
-            return getattr(module, obj)
-
     def __exit__(self, exc_type, exc_value, tb):
 
         if SKIP_IMPORT:
             self.failed_import = True
             return True
 
         silence_error = False
```

### Comparing `benchopt-1.3.1/benchopt/utils/shell_cmd.py` & `benchopt-1.4.0/benchopt/utils/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/slurm_executor.py` & `benchopt-1.4.0/benchopt/utils/slurm_executor.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/stream_redirection.py` & `benchopt-1.4.0/benchopt/utils/stream_redirection.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/sys_info.py` & `benchopt-1.4.0/benchopt/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/terminal_output.py` & `benchopt-1.4.0/benchopt/utils/terminal_output.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt/utils/tests/test_conda_env_cmd.py` & `benchopt-1.4.0/benchopt/utils/tests/test_conda_env_cmd.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/benchopt.egg-info/PKG-INFO` & `benchopt-1.4.0/benchopt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchopt
-Version: 1.3.1
+Version: 1.4.0
 Summary: Benchmark toolkit for optimization
 Download-URL: https://github.com/benchopt/benchopt.git
 Maintainer: Thomas Moreau
 Maintainer-email: thomas.moreau@inria.fr
 License: BSD (3-clause)
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -22,115 +22,159 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: slurm
 License-File: LICENSE
 
-Benchmark repository for optimization
-=====================================
+.. image:: https://raw.githubusercontent.com/benchopt/communication_materials/main/posters/images/logo_benchopt.png
+   :width: 350
+   :align: center
+   
+*—Making your optimization benchmarks simple and open—*
+
+----
 
-|Test Status| |Python 3.6+| |codecov|
+|Test Status| |codecov| |Python 3.6+| |install-per-months| |discord| |SWH|
 
-BenchOpt is a benchmarking suite for optimization algorithms.
+``Benchopt`` is a benchmarking suite for optimization algorithms.
 It is built for simplicity, transparency, and reproducibility.
+It is implemented in Python but can run algorithms written in **many programming languages**.
 
-Benchopt is implemented in Python, and can run algorithms
-written in **many programming languages**
-(`example <https://benchopt.github.io/auto_examples/plot_run_benchmark_python_R.html>`_).
-So far, Benchopt has been tested with `Python <https://www.python.org/>`_,
+
+So far, ``benchopt`` has been tested with `Python <https://www.python.org/>`_,
 `R <https://www.r-project.org/>`_, `Julia <https://julialang.org/>`_
 and `C/C++ <https://isocpp.org/>`_ (compiled binaries with a command line interface).
-Programs available via
-`conda <https://docs.conda.io/en/latest/>`_ should be compatible.
+Programs available via `conda <https://docs.conda.io/en/latest/>`_ should be compatible as well.
+See for instance an `example of usage <https://benchopt.github.io/auto_examples/plot_run_benchmark_python_R.html>`_ with ``R``.
 
-BenchOpt is run through a command line interface as described
-in the `API Documentation <https://benchopt.github.io/api.html>`_.
-Replicating an optimization benchmark should
-be **as simple as doing**:
 
-.. code-block::
 
-   conda create -n benchopt python
-   conda activate benchopt
-   pip install benchopt
-   git clone https://github.com/benchopt/benchmark_logreg_l2
-   cd benchmark_logreg_l2
-   benchopt install -e . -s lightning -s sklearn
-   benchopt run -e . --config ./example_config.yml
+Install
+-------
 
-Running this command will give you a benchmark plot on l2-regularized
-logistic regression:
+It is recommended to use ``benchopt`` within a ``conda`` environment to fully-benefit
+from ``benchopt`` Command Line Interface (CLI).  
 
-.. figure:: https://benchopt.github.io/_images/sphx_glr_plot_run_benchmark_001.png
-   :target: how.html
-   :align: center
-   :scale: 80%
 
-See the `Available optimization problems`_ below.
+To install ``benchopt``, start by creating a new ``conda`` environment and then activate it
 
-Learn how to `create a new benchmark <https://benchopt.github.io/how.html>`_
-using the `benchmark template <https://github.com/benchopt/template_benchmark>`_.
+.. code-block::
 
-Install
---------
+    conda create -n benchopt python
+    conda activate benchopt
 
-The command line tool to run the benchmarks can be installed through `pip`. In order to allow `benchopt`
-to automatically install solvers dependencies, the install needs to be done in a `conda` environment.
 
+Then run the following command to install the **latest release** of ``benchopt``
 
 .. code-block::
 
-    conda create -n benchopt python
-    conda activate benchopt
+    pip install -U benchopt
 
-To get the **latest release**, use:
+
+It is also possible to use the **latest development version**. To do so, run instead
 
 .. code-block::
 
-    pip install benchopt
+    pip install -U -i https://test.pypi.org/simple/benchopt
 
-To get the **latest development version**, use:
 
-.. code-block::
 
-    pip install -U -i https://test.pypi.org/simple/ benchopt
+Getting started 
+---------------
 
-Then, existing benchmarks can be retrieved from git or created locally.
-For instance, the benchmark for Lasso can be retrieved with:
+After installing ``benchopt``, you can
 
-.. code-block::
+- replicate/modify an existing benchmark
+- create your own benchmark
 
-    git clone https://github.com/benchopt/benchmark_lasso
 
+Using an existing benchmark
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-Command line interface
-----------------------
+Replicating an existing benchmark is simple.
+Here is how to do so for the `L2-logistic Regression benchmark <https://github.com/benchopt/benchmark_logreg_l2>`_.
 
-The preferred way to run the benchmarks is through the command line interface.
-To run the Lasso benchmark on all datasets and with all solvers, run:
+1. Clone the benchmark repository and ``cd`` to it
 
-.. code-block::
+.. code-block:: bash
 
-    benchopt run --env ./benchmark_lasso
+   git clone https://github.com/benchopt/benchmark_logreg_l2
+   cd benchmark_logreg_l2
 
-To get more details about the different options, run:
+2. Install the desired solvers automatically with ``benchopt``
 
-.. code-block::
+.. code-block:: bash
 
-    benchopt run -h
+   benchopt install . -s lightning -s sklearn
+
+3. Run the benchmark to get the figure below
+
+.. code-block:: bash
+
+   benchopt run . --config ./example_config.yml
+
+
+.. figure:: https://benchopt.github.io/_images/sphx_glr_plot_run_benchmark_001.png
+   :target: how.html
+   :align: center
+   :scale: 40%
 
-or read the `CLI documentation <https://benchopt.github.io/cli.html>`_.
 
-Benchopt also provides a Python API described in the
-`API documentation <https://benchopt.github.io/api.html>`_.
+These steps illustrate how to reproduce the `L2-logistic Regression benchmark <https://github.com/benchopt/benchmark_logreg_l2>`_.
+Find the complete list of the `Available benchmarks`_.
+Also, refer to the `documentation <https://benchopt.github.io/>`_ to learn more about ``benchopt`` CLI and its features.
+You can also easily extend this benchmark by adding a dataset, solver or metric.
+Learn that and more in the `Write a benchmark <https://benchopt.github.io/how.html>`_ tutorial.
 
 
-Available optimization problems
--------------------------------
+Creating a benchmark
+^^^^^^^^^^^^^^^^^^^^
+
+The section `Write a benchmark <https://benchopt.github.io/how.html>`_ of the documentation provides a tutorial
+for creating a benchmark. The ``benchopt`` community also maintains 
+a `template benchmark <https://github.com/benchopt/template_benchmark>`_ to quickly and easily start a new benchmark.
+
+
+
+Finding helps
+-------------
+
+Join ``benchopt`` `discord server <https://discord.gg/EA2HGQb7nv>`_ and get in touch with the community!
+Feel free to drop us a message to get help with running/constructing benchmarks 
+or (why not) discuss new features to be added and future development directions that ``benchopt`` should take.
+
+
+
+Citing Benchopt
+---------------
+
+``Benchopt`` is a continuous effort to make reproducible and transparent optimization benchmarks.
+Join us in this endeavor! If you use ``benchopt`` in a scientific publication, please cite
+
+.. code-block:: bibtex
+
+   @inproceedings{benchopt,
+      author    = {Moreau, Thomas and Massias, Mathurin and Gramfort, Alexandre 
+                   and Ablin, Pierre and Bannier, Pierre-Antoine 
+                   and Charlier, Benjamin and Dagréou, Mathieu and Dupré la Tour, Tom
+                   and Durif, Ghislain and F. Dantas, Cassio and Klopfenstein, Quentin
+                   and Larsson, Johan and Lai, En and Lefort, Tanguy 
+                   and Malézieux, Benoit and Moufad, Badr and T. Nguyen, Binh and Rakotomamonjy, 
+                   Alain and Ramzi, Zaccharie and Salmon, Joseph and Vaiter, Samuel},
+      title     = {Benchopt: Reproducible, efficient and collaborative optimization benchmarks},
+      year      = {2022},
+      booktitle = {NeurIPS},
+      url       = {https://arxiv.org/abs/2206.13424}
+   }
+
+
+
+Available benchmarks
+--------------------
 
 .. list-table::
    :widths: 70 15 15
    :header-rows: 1
 
    * - Problem
      - Results
@@ -144,77 +188,65 @@
    * - `LASSO: L1-Regularized Least Squares <https://github.com/benchopt/benchmark_lasso>`_
      - `Results <https://benchopt.github.io/results/benchmark_lasso.html>`__
      - |Build Status Lasso|
    * - `LASSO Path <https://github.com/jolars/benchmark_lasso_path>`_
      - `Results <https://benchopt.github.io/results/benchmark_lasso_path.html>`__
      - |Build Status Lasso Path|
    * - `Elastic Net <https://github.com/benchopt/benchmark_elastic_net>`_
-     - 
+     -
      - |Build Status ElasticNet|
    * - `MCP <https://github.com/benchopt/benchmark_mcp>`_
      - `Results <https://benchopt.github.io/results/benchmark_mcp.html>`__
      - |Build Status MCP|
    * - `L2-Regularized Logistic Regression <https://github.com/benchopt/benchmark_logreg_l2>`_
      - `Results <https://benchopt.github.io/results/benchmark_logreg_l2.html>`__
      - |Build Status LogRegL2|
    * - `L1-Regularized Logistic Regression <https://github.com/benchopt/benchmark_logreg_l1>`_
      - `Results <https://benchopt.github.io/results/benchmark_logreg_l1.html>`__
      - |Build Status LogRegL1|
    * - `L2-regularized Huber regression <https://github.com/benchopt/benchmark_huber_l2>`_
-     - 
+     -
      - |Build Status HuberL2|
    * - `L1-Regularized Quantile Regression <https://github.com/benchopt/benchmark_quantile_regression>`_
      - `Results <https://benchopt.github.io/results/benchmark_quantile_regression.html>`__
      - |Build Status QuantileRegL1|
    * - `Linear SVM for Binary Classification <https://github.com/benchopt/benchmark_linear_svm_binary_classif_no_intercept>`_
-     - 
+     -
      - |Build Status LinearSVM|
    * - `Linear ICA <https://github.com/benchopt/benchmark_linear_ica>`_
-     - 
+     -
      - |Build Status LinearICA|
    * - `Approximate Joint Diagonalization (AJD) <https://github.com/benchopt/benchmark_jointdiag>`_
-     - 
+     -
      - |Build Status JointDiag|
    * - `1D Total Variation Denoising <https://github.com/benchopt/benchmark_tv_1d>`_
      -
      - |Build Status TV1D|
    * - `2D Total Variation Denoising <https://github.com/benchopt/benchmark_tv_2d>`_
-     - 
+     -
      - |Build Status TV2D|
    * - `ResNet Classification <https://github.com/benchopt/benchmark_resnet_classif>`_
      - `Results <https://benchopt.github.io/results/benchmark_resnet_classif.html>`__
      - |Build Status ResNetClassif|
 
 
-Citing Benchopt
----------------
-
-If you use ``Benchopt`` in a scientific publication, please cite the following paper
-
-.. code-block:: bibtex
-
-   @article{benchopt,
-      author = {Moreau, Thomas and Massias, Mathurin and Gramfort, Alexandre and Ablin, Pierre 
-                and Bannier, Pierre-Antoine and Charlier, Benjamin and Dagréou, Mathieu and Dupré la Tour, Tom 
-                and Durif, Ghislain and F. Dantas, Cassio and Klopfenstein, Quentin 
-                and Larsson, Johan and Lai, En and Lefort, Tanguy and Malézieux, Benoit 
-                and Moufad, Badr and T. Nguyen, Binh and Rakotomamonjy, Alain and Ramzi, Zaccharie 
-                and Salmon, Joseph and Vaiter, Samuel},
-      title  = {Benchopt: Reproducible, efficient and collaborative optimization benchmarks},
-      year   = {2022},
-      url    = {https://arxiv.org/abs/2206.13424}
-   }
 
 
 .. |Test Status| image:: https://github.com/benchopt/benchopt/actions/workflows/test.yml/badge.svg
    :target: https://github.com/benchopt/benchopt/actions/workflows/test.yml
 .. |Python 3.6+| image:: https://img.shields.io/badge/python-3.6%2B-blue
    :target: https://www.python.org/downloads/release/python-360/
 .. |codecov| image:: https://codecov.io/gh/benchopt/benchopt/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/benchopt/benchopt
+.. |SWH| image:: https://archive.softwareheritage.org/badge/origin/https://github.com/benchopt/benchopt/
+    :target: https://archive.softwareheritage.org/browse/origin/?origin_url=https://github.com/benchopt/benchopt
+.. |discord| image:: https://dcbadge.vercel.app/api/server/EA2HGQb7nv?style=flat
+   :target: https://discord.gg/EA2HGQb7nv
+.. |install-per-months| image:: https://static.pepy.tech/badge/benchopt/month
+   :target: https://pepy.tech/project/benchopt
 
 .. |Build Status OLS| image:: https://github.com/benchopt/benchmark_ols/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_ols/actions
 .. |Build Status NNLS| image:: https://github.com/benchopt/benchmark_nnls/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_nnls/actions
 .. |Build Status Lasso| image:: https://github.com/benchopt/benchmark_lasso/workflows/Tests/badge.svg
    :target: https://github.com/benchopt/benchmark_lasso/actions
```

### Comparing `benchopt-1.3.1/benchopt.egg-info/SOURCES.txt` & `benchopt-1.4.0/benchopt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,25 @@
 continuous_integration/build_doc.sh
 continuous_integration/install_coverage_subprocess_pth.py
 continuous_integration/test_req_detection.sh
 continuous_integration/test_script.sh
 doc/Makefile
 doc/advanced.rst
 doc/api.rst
+doc/benchmark_list.rst
 doc/cli.rst
 doc/conf.py
 doc/config.rst
 doc/contrib.rst
 doc/how.rst
 doc/index.rst
 doc/names.inc
+doc/performance_curves.rst
 doc/publish.rst
+doc/test_config.rst
 doc/whats_new.rst
 doc/_static/github_benchopt_token.png
 doc/_static/style.css
 doc/_templates/search.html
 doc/_templates/autosummary/class.rst
 doc/_templates/autosummary/function.rst
 doc/sphinxext/gh_substitutions.py
```

### Comparing `benchopt-1.3.1/continuous_integration/test_req_detection.sh` & `benchopt-1.4.0/continuous_integration/test_req_detection.sh`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/continuous_integration/test_script.sh` & `benchopt-1.4.0/continuous_integration/test_script.sh`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/Makefile` & `benchopt-1.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/_static/github_benchopt_token.png` & `benchopt-1.4.0/doc/_static/github_benchopt_token.png`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/_static/style.css` & `benchopt-1.4.0/doc/_static/style.css`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/_templates/search.html` & `benchopt-1.4.0/doc/_templates/search.html`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/advanced.rst` & `benchopt-1.4.0/doc/advanced.rst`

 * *Files 24% similar despite different names*

```diff
@@ -95,26 +95,27 @@
 
             return False, None
 
 
 
 .. _sampling_strategy:
 
-Changing the strategy to grow the :code:`stop_val`
---------------------------------------------------
+Changing the strategy to grow the computational budget (:code:`stop_val`)
+------------------------------------------------------------------------
 
-By default, the number of iterations or the variation of the tolerance
-between  two evaluations of the objective is exponential. However, in
-some cases, this exponential growth might hide some effects, or might
-not be adapted to a given solver.
+Benchopt varies the computational budget by varying either the number
+of iterations or the tolerance given to the method. The default policy is
+to vary these two quantities exponentially between two evaluations of the
+objective. However, in some cases, this exponential growth might hide some
+effects, or might not be adapted to a given solver.
 
 The way this value is changed can be specified for each solver by
-implementing the ``get_next`` method in the ``Solver`` class.
+implementing a ``get_next`` method in the ``Solver`` class.
 This method takes as input the previous value where the objective
-function have been logged, and output the next one. For instance,
+function has been logged, and outputs the next one. For instance,
 if a solver needs to be evaluated every 10 iterations, we would have
 
 .. code-block::
 
     class Solver(BaseSolver):
         ...
         def get_next(self, stop_val):
@@ -155,12 +156,43 @@
 
     with safe_import_context() as import_ctx:
         from benchmark_utils import helper1
         from benchmark_utils.helper1 import func1
         from benchmark_utils.helper_module.submodule1 import func2
 
 
+
+.. _precompilation:
+
+Caching pre-compilation and warmup effects
+------------------------------------------
+
+For some solvers, such as solver relying on just-in-time compilation with
+``numba`` or ``jax``, the first iteration might be longer due to "warmup"
+effects. To avoid having such effect in the benchmark results, it is usually
+advised to call the solver once before running the benchmark, in the
+``Solver.set_objective`` method. For solvers with ``stopping_strategy`` in
+``{'tolerance',  'iteration'}``, simply calling the ``Solver.run`` with a
+simple enough value is usually enough. For solvers with ``stopping_strategy``
+set to ``'callback'``, it is possible to call ``Solver.run_once``, which will
+call the ``run`` method with a simple callback that does not compute the
+objective value and stops after ``n_iter`` calls to callback (default to 1).
+
+
+.. code-block:: python
+
+    class Solver(BaseSolver):
+        ...
+
+        def set_objective(self, **objective):
+            ...
+            # Cache pre-compilation and other one-time setups that should
+            # not be included in the benchmark timing.
+            self.run(1)  # For stopping_strategy == 'iteration' | 'tolerance'
+            self.run_once()  # For stopping_strategy == 'callback'
+
+
 .. |update_params| replace:: ``update_parameters``
 .. _update_params: https://github.com/facebookincubator/submitit/blob/main/submitit/slurm/slurm.py#L386
 
 .. |SlurmExecutor| replace:: ``submitit.SlurmExecutor``
-.. _SlurmExecutor: https://github.com/facebookincubator/submitit/blob/main/submitit/slurm/slurm.py#L214
+.. _SlurmExecutor: https://github.com/facebookincubator/submitit/blob/main/submitit/slurm/slurm.py#L214
```

### Comparing `benchopt-1.3.1/doc/cli.rst` & `benchopt-1.4.0/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/conf.py` & `benchopt-1.4.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/config.rst` & `benchopt-1.4.0/doc/config.rst`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/contrib.rst` & `benchopt-1.4.0/doc/contrib.rst`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/how.rst` & `benchopt-1.4.0/doc/how.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 as for `Ordinary Least Square (OLS) <https://github.com/benchopt/benchmark_ols>`_,
 `Lasso <https://github.com/benchopt/benchmark_lasso>`_ or
 `L1-regularized logistic regression <https://github.com/benchopt/benchmark_logreg_l1>`_.
 
 .. note::
 
     The simplest way to create a benchmark is to copy an existing folder and
-    modify the element to fit the new structure.
+    to adapt its content.
     A benchmark template is provided as a `GitHub template repo here <https://github.com/benchopt/template_benchmark>`_
 
 
 .. _objective:
 
 1. Objective
 ------------
@@ -56,15 +56,15 @@
   is returned it should contain a key called ``value`` (the objective value) and all other keys
   should have ``float`` values allowing to track more than one value
   of interest (e.g. train and test errors).
 - ``get_objective()``: method that returns a dictionary to be passed
   to the ``set_objective`` methods of solvers_.
 
 An objective class also needs to inherit from a base class,
-:class:`benchopt.base.BaseObjective`.
+:class:`benchopt.BaseObjective`.
 
 .. note::
   Multiple values can be computed in one objective as long as they are
   stored in a dictionary with a key being ``value``. This allows to compute
   different metrics at once.
 
 Example
@@ -76,18 +76,16 @@
 
 2. Datasets
 -----------
 
 A dataset defines what can be passed to an objective. More specifically,
 a dataset should implement one method:
 
-   - ``get_data()``: A method whose output consists of two things. First it outputs
-     the dimension of the optimization problem (size of the iterates). Second it
-     outputs a dictionary that can be passed as keyword arguments ``**data`` to
-     the ``set_data`` method of an objective_.
+- ``get_data()``: A method which outputs a dictionary that can be passed as
+  keyword arguments ``**data`` to the ``set_data`` method of an objective_.
 
 A dataset class also needs to inherit from a base class called
 :class:`benchopt.BaseDataset`.
 
 Example using a real dataset
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `benchopt-1.3.1/doc/names.inc` & `benchopt-1.4.0/doc/names.inc`

 * *Files 4% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 
 .. _Ghislain Durif: https://gdurif.perso.math.cnrs.fr/
 
 .. _Benoît Malézieux: https://github.com/bmalezieux
 
 .. _Amélie Vernay: https://github.com/AmelieVernay
 
-.. _Melvine Nargeot: https://github.com/Melvin-klein
+.. _Melvine Nargeot: https://github.com/Melvin-klein
+
+.. _Badr Moufad: https://github.com/Badr-MOUFAD
```

### Comparing `benchopt-1.3.1/doc/publish.rst` & `benchopt-1.4.0/doc/publish.rst`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/sphinxext/gh_substitutions.py` & `benchopt-1.4.0/doc/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/sphinxext/sphinx_click_semantic_group.py` & `benchopt-1.4.0/doc/sphinxext/sphinx_click_semantic_group.py`

 * *Files identical despite different names*

### Comparing `benchopt-1.3.1/doc/whats_new.rst` & `benchopt-1.4.0/doc/whats_new.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,68 @@
 .. _whats_new:
 
 What's new
 ==========
 
 .. currentmodule:: benchopt
 
+.. _changes_1_4:
+
+Version 1.4 - 03/07/2023
+------------------------
+
+CLI
+~~~
+
+- Add support for minute and hour unit suffix in timeout limit through the syntax
+  ``--timeout 10m`` or ``--timeout 1h``.
+  By `Mathurin Massias`_ (:gh:`535`).
+- Remove deprecated ``-o/--objective-filter`` option in ``benchopt run``.
+  By `Thomas Moreau`_ (:gh:`569`)
+
+
+API
+~~~
+
+- The ``get_next`` method of :class:`~benchopt.BaseSolver` is no longer static.
+  By `Badr Moufad`_ (:gh:`566`)
+
+- Add :class:`~benchopt.stopping_criterion.SingleRunCriterion` to run a solver
+  only once. This can be used for benchmarking methods where we are interested
+  in objective value at convergence. By `Thomas Moreau`_ (:gh:`511`)
+
+- Add :func:`~benchopt.BaseSolver.run_once` helper to easily warmup solvers
+  with callback. By `Thomas Moreau`_ (:gh:`511`)
+
+- Add :func:`~benchopt.BaseSolver.pre_run_hook` hook to ignore cost that cannot
+  be cached globally for a solver. By `Thomas Moreau`_ (:gh:`525`)
+
+- Remove deprecated ``Objective.to_dict``, ``safe_import_context.import_from``.
+  Force implementation of :method:`benchopt.Objective.get_one_solution`.
+  By `Thomas Moreau`_ (:gh:`569`)
+
+PLOT
+~~~~
+
+- Add a tooltip beside to show description of objective. Description is provided as docstring of
+  the :class:`~benchopt.BaseObjective` class. By `Badr Moufad`_ (:gh:`556`)
+
+- Show solver description when hovering over solvers. Description is provided as docstring of
+  the :class:`~benchopt.BaseSolver` class. By `Badr Moufad`_ (:gh:`543`)
+
+- Enable visualizing the objective as function of ``stopping_criterion``: time,
+  iteration, or tolerance. By `Badr Moufad`_ (:gh:`479`)
+
+FIX
+~~~
+
+- Do not fail and raise a warning when ``safe_import_context`` is not named
+  ``import_ctx``. By `Mathurin Massias`_ (:gh:`524`)
+
+
 .. _changes_1_3_1:
 
 Version 1.3.1 - 01/12/2022
 --------------------------
 
 Bug fix release
```

### Comparing `benchopt-1.3.1/examples/plot_run_benchmark.py` & `benchopt-1.4.0/examples/plot_run_benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 from pathlib import Path
 import matplotlib.pyplot as plt
 from benchopt import run_benchmark
 from benchopt.benchmark import Benchmark
 from benchopt.plotting import plot_benchmark, PLOT_KINDS
+from benchopt.plotting.plot_objective_curve import reset_solver_styles_idx
 
 
 BENCHMARK_PATH = (
     Path().resolve().parent / 'benchmarks' / 'benchmark_logreg_l2'
 )
 
 
@@ -33,10 +34,11 @@
         "`benchmarks` folder. Please run:\n"
         "$ git clone https://github.com/benchopt/benchmark_logreg_l2 "
         f"{BENCHMARK_PATH.resolve()}"
     )
 
 
 kinds = list(PLOT_KINDS.keys())
+reset_solver_styles_idx()
 figs = plot_benchmark(save_file, benchmark=Benchmark(BENCHMARK_PATH),
                       kinds=kinds, html=False)
 plt.show()
```

### Comparing `benchopt-1.3.1/examples/plot_run_benchmark_python_R.py` & `benchopt-1.4.0/examples/plot_run_benchmark_python_R.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 from pathlib import Path
 import matplotlib.pyplot as plt
 from benchopt import run_benchmark
 from benchopt.benchmark import Benchmark
 from benchopt.plotting import plot_benchmark, PLOT_KINDS
+from benchopt.plotting.plot_objective_curve import reset_solver_styles_idx
 
 
 BENCHMARK_PATH = Path().resolve().parent / 'benchmarks' / 'benchmark_lasso'
 
 if not BENCHMARK_PATH.exists():
     raise RuntimeError(
         "This example can only work when Lasso benchmark is cloned in the "
@@ -29,10 +30,11 @@
     objective_filters=['*[fit_intercept=False,reg=0.5]'],
     max_runs=100, timeout=100, n_repetitions=5,
     plot_result=False, show_progress=False
 )
 
 
 kinds = list(PLOT_KINDS.keys())
+reset_solver_styles_idx()
 figs = plot_benchmark(save_file, benchmark=Benchmark(BENCHMARK_PATH),
                       kinds=kinds, html=False)
 plt.show()
```

### Comparing `benchopt-1.3.1/pyproject.toml` & `benchopt-1.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   "setuptools_scm>=6.2"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "benchopt/version.py"
 local_scheme = "no-local-version"
-fallback_version = "dev"
+fallback_version = "99.0.dev0"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-v -p benchopt.tests.fixtures"
 testpaths = [
     "benchopt",
 ]
```

### Comparing `benchopt-1.3.1/roadmap.md` & `benchopt-1.4.0/roadmap.md`

 * *Files 14% similar despite different names*

```diff
@@ -21,7 +21,13 @@
 ## Current TODO:
 
 - [ ] Adapt n_iter spacing to time (while loop)
 - [ ] Compute optimal solution
 - [ ] Argument in client to pass solvers to run in benchmark
 - [ ] Make CI run the benchmark and check install
 
+
+## Discussion Owkin
+
+- Checkpointing is important.
+- Merging files from multiple run?
+
```

### Comparing `benchopt-1.3.1/setup.cfg` & `benchopt-1.4.0/setup.cfg`

 * *Files identical despite different names*

