# Comparing `tmp/etna-2.0.0.tar.gz` & `tmp/etna-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etna-2.0.0.tar", max compression
+gzip compressed data, was "etna-2.1.0.tar", max compression
```

## Comparing `etna-2.0.0.tar` & `etna-2.1.0.tar`

### file list

```diff
@@ -1,197 +1,204 @@
--rw-r--r--   0        0        0    11244 2023-04-12 06:09:53.967157 etna-2.0.0/LICENSE
--rw-r--r--   0        0        0    13188 2023-04-12 06:09:53.971157 etna-2.0.0/README.md
--rw-r--r--   0        0        0       49 2023-04-12 06:09:53.971157 etna-2.0.0/etna/__init__.py
--rw-r--r--   0        0        0     2388 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/__init__.py
--rw-r--r--   0        0        0      599 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/__init__.py
--rw-r--r--   0        0        0    16581 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/plots.py
--rw-r--r--   0        0        0     1189 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/search.py
--rw-r--r--   0        0        0     9835 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/decomposition/utils.py
--rw-r--r--   0        0        0      475 2023-04-12 06:09:53.971157 etna-2.0.0/etna/analysis/eda/__init__.py
--rw-r--r--   0        0        0    26025 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/eda/plots.py
--rw-r--r--   0        0        0     4077 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/eda/utils.py
--rw-r--r--   0        0        0      472 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/__init__.py
--rw-r--r--   0        0        0     6004 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/plots.py
--rw-r--r--   0        0        0     3114 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/relevance.py
--rw-r--r--   0        0        0     3962 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/relevance_table.py
--rw-r--r--   0        0        0      654 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_relevance/utils.py
--rw-r--r--   0        0        0      213 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_selection/__init__.py
--rw-r--r--   0        0        0     3870 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/feature_selection/mrmr_selection.py
--rw-r--r--   0        0        0      737 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/forecast/__init__.py
--rw-r--r--   0        0        0    35388 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/forecast/plots.py
--rw-r--r--   0        0        0     3855 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/forecast/utils.py
--rw-r--r--   0        0        0      517 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/__init__.py
--rw-r--r--   0        0        0     4879 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/density_outliers.py
--rw-r--r--   0        0        0    13169 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/hist_outliers.py
--rw-r--r--   0        0        0     1739 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/median_outliers.py
--rw-r--r--   0        0        0     5343 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/plots.py
--rw-r--r--   0        0        0     3131 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/outliers/prediction_interval_outliers.py
--rw-r--r--   0        0        0     1471 2023-04-12 06:09:53.975157 etna-2.0.0/etna/analysis/utils.py
--rw-r--r--   0        0        0       64 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/__init__.py
--rw-r--r--   0        0        0    12482 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/auto.py
--rw-r--r--   0        0        0      102 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/optuna/__init__.py
--rw-r--r--   0        0        0     4680 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/optuna/config_sampler.py
--rw-r--r--   0        0        0     2828 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/optuna/wrapper.py
--rw-r--r--   0        0        0       93 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/generator.py
--rw-r--r--   0        0        0     5348 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/templates.py
--rw-r--r--   0        0        0      495 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/pool/utils.py
--rw-r--r--   0        0        0      151 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/__init__.py
--rw-r--r--   0        0        0      451 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/base.py
--rw-r--r--   0        0        0     2114 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/local.py
--rw-r--r--   0        0        0      171 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/runner/utils.py
--rw-r--r--   0        0        0      740 2023-04-12 06:09:53.975157 etna-2.0.0/etna/auto/utils.py
--rw-r--r--   0        0        0      524 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/__init__.py
--rw-r--r--   0        0        0      686 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/base.py
--rw-r--r--   0        0        0      259 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/__init__.py
--rw-r--r--   0        0        0     3756 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/base.py
--rw-r--r--   0        0        0     4508 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/distance_matrix.py
--rw-r--r--   0        0        0     5597 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/dtw_distance.py
--rw-r--r--   0        0        0     1705 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/distances/euclidean_distance.py
--rw-r--r--   0        0        0      289 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/base.py
--rw-r--r--   0        0        0     1501 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/dtw_clustering.py
--rw-r--r--   0        0        0     1561 2023-04-12 06:09:53.975157 etna-2.0.0/etna/clustering/hierarchical/euclidean_clustering.py
--rw-r--r--   0        0        0      374 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/__init__.py
--rw-r--r--   0        0        0      197 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/__main__.py
--rw-r--r--   0        0        0     3549 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/backtest_command.py
--rw-r--r--   0        0        0     3858 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/forecast_command.py
--rw-r--r--   0        0        0      281 2023-04-12 06:09:53.975157 etna-2.0.0/etna/commands/resolvers.py
--rw-r--r--   0        0        0      205 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/__init__.py
--rw-r--r--   0        0        0     9194 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/mixins.py
--rw-r--r--   0        0        0      617 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/saving.py
--rw-r--r--   0        0        0     2248 2023-04-12 06:09:53.975157 etna-2.0.0/etna/core/utils.py
--rw-r--r--   0        0        0      548 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/__init__.py
--rw-r--r--   0        0        0     8274 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/datasets_generation.py
--rw-r--r--   0        0        0     7778 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/hierarchical_structure.py
--rw-r--r--   0        0        0    61946 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/tsdataset.py
--rw-r--r--   0        0        0    10283 2023-04-12 06:09:53.975157 etna-2.0.0/etna/datasets/utils.py
--rw-r--r--   0        0        0      226 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/__init__.py
--rw-r--r--   0        0        0     6197 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/direct_ensemble.py
--rw-r--r--   0        0        0     4671 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/mixins.py
--rw-r--r--   0        0        0    10931 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/stacking_ensemble.py
--rw-r--r--   0        0        0     9437 2023-04-12 06:09:53.975157 etna-2.0.0/etna/ensembles/voting_ensemble.py
--rw-r--r--   0        0        0       94 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/change_points/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/change_points/regularization_search.py
--rw-r--r--   0        0        0      170 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/__init__.py
--rw-r--r--   0        0        0      473 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/base.py
--rw-r--r--   0        0        0     4926 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/classification.py
--rw-r--r--   0        0        0      290 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/__init__.py
--rw-r--r--   0        0        0     1543 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/base.py
--rw-r--r--   0        0        0     2503 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/tsfresh.py
--rw-r--r--   0        0        0    14997 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/feature_extraction/weasel.py
--rw-r--r--   0        0        0     3241 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/predictability.py
--rw-r--r--   0        0        0      874 2023-04-12 06:09:53.975157 etna-2.0.0/etna/experimental/classification/utils.py
--rw-r--r--   0        0        0        0 2023-04-12 06:09:53.975157 etna-2.0.0/etna/libs/__init__.py
--rw-r--r--   0        0        0       79 2023-04-12 06:09:53.975157 etna-2.0.0/etna/libs/pmdarima_utils/__init__.py
--rw-r--r--   0        0        0     7455 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pmdarima_utils/arima.py
--rw-r--r--   0        0        0      415 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pmdarima_utils/arima.pyi
--rw-r--r--   0        0        0        0 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      472 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/pytorch_lightning/callbacks.py
--rw-r--r--   0        0        0      341 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/__init__.py
--rw-r--r--   0        0        0     1745 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/defaults.py
--rw-r--r--   0        0        0     1831 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/distribution.py
--rw-r--r--   0        0        0       69 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/distribution.pyi
--rw-r--r--   0        0        0    16540 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/relevance.py
--rw-r--r--   0        0        0      823 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/relevance.pyi
--rw-r--r--   0        0        0     8431 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/significance_tests.py
--rw-r--r--   0        0        0      344 2023-04-12 06:09:53.979157 etna-2.0.0/etna/libs/tsfresh/significance_tests.pyi
--rw-r--r--   0        0        0      804 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/__init__.py
--rw-r--r--   0        0        0     4993 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/base.py
--rw-r--r--   0        0        0     2643 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/console_logger.py
--rw-r--r--   0        0        0    15306 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/file_logger.py
--rw-r--r--   0        0        0     7105 2023-04-12 06:09:53.979157 etna-2.0.0/etna/loggers/wandb_logger.py
--rw-r--r--   0        0        0     1230 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/__init__.py
--rw-r--r--   0        0        0     7625 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/base.py
--rw-r--r--   0        0        0     5151 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/functional_metrics.py
--rw-r--r--   0        0        0     5513 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/intervals_metrics.py
--rw-r--r--   0        0        0     9643 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/metrics.py
--rw-r--r--   0        0        0     2539 2023-04-12 06:09:53.979157 etna-2.0.0/etna/metrics/utils.py
--rw-r--r--   0        0        0     1729 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/__init__.py
--rw-r--r--   0        0        0     2521 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/autoarima.py
--rw-r--r--   0        0        0    22815 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/base.py
--rw-r--r--   0        0        0    14654 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/catboost.py
--rw-r--r--   0        0        0    13704 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/deadline_ma.py
--rw-r--r--   0        0        0      557 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/decorators.py
--rw-r--r--   0        0        0    30566 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/holt_winters.py
--rw-r--r--   0        0        0     7136 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/linear.py
--rw-r--r--   0        0        0    22799 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/mixins.py
--rw-r--r--   0        0        0      828 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/moving_average.py
--rw-r--r--   0        0        0      712 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/naive.py
--rw-r--r--   0        0        0      307 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/__init__.py
--rw-r--r--   0        0        0     9210 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/deepar.py
--rw-r--r--   0        0        0     7988 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/mlp.py
--rw-r--r--   0        0        0    10502 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/rnn.py
--rw-r--r--   0        0        0    10658 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/tft.py
--rw-r--r--   0        0        0    11824 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/nn/utils.py
--rw-r--r--   0        0        0    18870 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/prophet.py
--rw-r--r--   0        0        0    31892 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/sarimax.py
--rw-r--r--   0        0        0     8465 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/seasonal_ma.py
--rw-r--r--   0        0        0     3555 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/sklearn.py
--rw-r--r--   0        0        0    19716 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/tbats.py
--rw-r--r--   0        0        0     3685 2023-04-12 06:09:53.979157 etna-2.0.0/etna/models/utils.py
--rw-r--r--   0        0        0      292 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/__init__.py
--rw-r--r--   0        0        0     5437 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/assembling_pipelines.py
--rw-r--r--   0        0        0     7232 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/autoregressive_pipeline.py
--rw-r--r--   0        0        0    36768 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/base.py
--rw-r--r--   0        0        0    14014 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/hierarchical_pipeline.py
--rw-r--r--   0        0        0     7388 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/mixins.py
--rw-r--r--   0        0        0     5467 2023-04-12 06:09:53.979157 etna-2.0.0/etna/pipeline/pipeline.py
--rw-r--r--   0        0        0        0 2023-04-12 06:09:53.979157 etna-2.0.0/etna/py.typed
--rw-r--r--   0        0        0      181 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/__init__.py
--rw-r--r--   0        0        0     3473 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/base.py
--rw-r--r--   0        0        0     1899 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/bottom_up.py
--rw-r--r--   0        0        0     5742 2023-04-12 06:09:53.979157 etna-2.0.0/etna/reconciliation/top_down.py
--rw-r--r--   0        0        0     9971 2023-04-12 06:09:53.979157 etna-2.0.0/etna/settings.py
--rw-r--r--   0        0        0     3234 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/__init__.py
--rw-r--r--   0        0        0    12526 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/base.py
--rw-r--r--   0        0        0     1168 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/__init__.py
--rw-r--r--   0        0        0      949 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/__init__.py
--rw-r--r--   0        0        0     7980 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/base.py
--rw-r--r--   0        0        0      250 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
--rw-r--r--   0        0        0     1886 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
--rw-r--r--   0        0        0     2171 2023-04-12 06:09:53.979157 etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
--rw-r--r--   0        0        0     3600 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/detrend.py
--rw-r--r--   0        0        0     3080 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/level.py
--rw-r--r--   0        0        0      887 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
--rw-r--r--   0        0        0      724 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
--rw-r--r--   0        0        0     1311 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
--rw-r--r--   0        0        0     3397 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
--rw-r--r--   0        0        0     2496 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
--rw-r--r--   0        0        0     3445 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/segmentation.py
--rw-r--r--   0        0        0     3369 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/change_points_based/trend.py
--rw-r--r--   0        0        0     7358 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/detrend.py
--rw-r--r--   0        0        0     7670 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/decomposition/stl.py
--rw-r--r--   0        0        0      306 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/__init__.py
--rw-r--r--   0        0        0     6985 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/categorical.py
--rw-r--r--   0        0        0     2836 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/mean_segment_encoder.py
--rw-r--r--   0        0        0     2525 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/encoders/segment_encoder.py
--rw-r--r--   0        0        0      444 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/__init__.py
--rw-r--r--   0        0        0     2469 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/base.py
--rw-r--r--   0        0        0     7308 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/feature_importance.py
--rw-r--r--   0        0        0     3434 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/filter.py
--rw-r--r--   0        0        0    14261 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/feature_selection/gale_shapley.py
--rw-r--r--   0        0        0     1326 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/__init__.py
--rw-r--r--   0        0        0     4821 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/add_constant.py
--rw-r--r--   0        0        0     5645 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/apply_lambda.py
--rw-r--r--   0        0        0    16679 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/differencing.py
--rw-r--r--   0        0        0     3346 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/lags.py
--rw-r--r--   0        0        0     5002 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/log.py
--rw-r--r--   0        0        0     3330 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/power.py
--rw-r--r--   0        0        0     8464 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/scalers.py
--rw-r--r--   0        0        0    11348 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/sklearn.py
--rw-r--r--   0        0        0    21230 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/math/statistics.py
--rw-r--r--   0        0        0      233 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/missing_values/__init__.py
--rw-r--r--   0        0        0     9100 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/missing_values/imputation.py
--rw-r--r--   0        0        0     6698 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/missing_values/resample.py
--rw-r--r--   0        0        0      301 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/outliers/__init__.py
--rw-r--r--   0        0        0     5106 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/outliers/base.py
--rw-r--r--   0        0        0     5733 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/outliers/point_outliers.py
--rw-r--r--   0        0        0      334 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/__init__.py
--rw-r--r--   0        0        0    14352 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/date_flags.py
--rw-r--r--   0        0        0     5135 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/fourier.py
--rw-r--r--   0        0        0     2848 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/holiday.py
--rw-r--r--   0        0        0     8370 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/special_days.py
--rw-r--r--   0        0        0     8347 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/timestamp/time_flags.py
--rw-r--r--   0        0        0      734 2023-04-12 06:09:53.983157 etna-2.0.0/etna/transforms/utils.py
--rw-r--r--   0        0        0    11759 2023-04-12 06:09:54.147159 etna-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    18682 1970-01-01 00:00:00.000000 etna-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11244 2023-07-03 15:27:34.976775 etna-2.1.0/LICENSE
+-rw-r--r--   0        0        0    13778 2023-07-03 15:27:34.976775 etna-2.1.0/README.md
+-rw-r--r--   0        0        0       49 2023-07-03 15:27:34.980775 etna-2.1.0/etna/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/__init__.py
+-rw-r--r--   0        0        0    16581 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/plots.py
+-rw-r--r--   0        0        0     1189 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/search.py
+-rw-r--r--   0        0        0     9835 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/decomposition/utils.py
+-rw-r--r--   0        0        0      475 2023-07-03 15:27:34.980775 etna-2.1.0/etna/analysis/eda/__init__.py
+-rw-r--r--   0        0        0    26025 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/eda/plots.py
+-rw-r--r--   0        0        0     4113 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/eda/utils.py
+-rw-r--r--   0        0        0      472 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/__init__.py
+-rw-r--r--   0        0        0     6004 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/plots.py
+-rw-r--r--   0        0        0     3114 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/relevance.py
+-rw-r--r--   0        0        0     4116 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/relevance_table.py
+-rw-r--r--   0        0        0      654 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_relevance/utils.py
+-rw-r--r--   0        0        0      213 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_selection/__init__.py
+-rw-r--r--   0        0        0     5023 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/feature_selection/mrmr_selection.py
+-rw-r--r--   0        0        0      737 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/forecast/__init__.py
+-rw-r--r--   0        0        0    35626 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/forecast/plots.py
+-rw-r--r--   0        0        0     4142 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/forecast/utils.py
+-rw-r--r--   0        0        0      517 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/__init__.py
+-rw-r--r--   0        0        0     4879 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/density_outliers.py
+-rw-r--r--   0        0        0    13169 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/hist_outliers.py
+-rw-r--r--   0        0        0     1739 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/median_outliers.py
+-rw-r--r--   0        0        0     5343 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/plots.py
+-rw-r--r--   0        0        0     3878 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/outliers/prediction_interval_outliers.py
+-rw-r--r--   0        0        0     1471 2023-07-03 15:27:34.984775 etna-2.1.0/etna/analysis/utils.py
+-rw-r--r--   0        0        0       96 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/__init__.py
+-rw-r--r--   0        0        0    31738 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/auto.py
+-rw-r--r--   0        0        0      102 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/optuna/__init__.py
+-rw-r--r--   0        0        0     4737 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/optuna/config_sampler.py
+-rw-r--r--   0        0        0     2828 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/optuna/wrapper.py
+-rw-r--r--   0        0        0       93 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/__init__.py
+-rw-r--r--   0        0        0     1533 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/generator.py
+-rw-r--r--   0        0        0     5348 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/templates.py
+-rw-r--r--   0        0        0      495 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/pool/utils.py
+-rw-r--r--   0        0        0      151 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/__init__.py
+-rw-r--r--   0        0        0      451 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/base.py
+-rw-r--r--   0        0        0     2114 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/local.py
+-rw-r--r--   0        0        0      171 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/runner/utils.py
+-rw-r--r--   0        0        0     1664 2023-07-03 15:27:34.984775 etna-2.1.0/etna/auto/utils.py
+-rw-r--r--   0        0        0      524 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/base.py
+-rw-r--r--   0        0        0      259 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/__init__.py
+-rw-r--r--   0        0        0     3756 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/base.py
+-rw-r--r--   0        0        0     4508 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/distance_matrix.py
+-rw-r--r--   0        0        0     5597 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/dtw_distance.py
+-rw-r--r--   0        0        0     1705 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/distances/euclidean_distance.py
+-rw-r--r--   0        0        0      289 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/__init__.py
+-rw-r--r--   0        0        0     6025 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/base.py
+-rw-r--r--   0        0        0     1501 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/dtw_clustering.py
+-rw-r--r--   0        0        0     1561 2023-07-03 15:27:34.984775 etna-2.1.0/etna/clustering/hierarchical/euclidean_clustering.py
+-rw-r--r--   0        0        0      374 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/__main__.py
+-rw-r--r--   0        0        0     4832 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/backtest_command.py
+-rw-r--r--   0        0        0     6885 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/forecast_command.py
+-rw-r--r--   0        0        0      281 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/resolvers.py
+-rw-r--r--   0        0        0     4415 2023-07-03 15:27:34.984775 etna-2.1.0/etna/commands/utils.py
+-rw-r--r--   0        0        0      205 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/__init__.py
+-rw-r--r--   0        0        0    11102 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/mixins.py
+-rw-r--r--   0        0        0      631 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/saving.py
+-rw-r--r--   0        0        0     2248 2023-07-03 15:27:34.984775 etna-2.1.0/etna/core/utils.py
+-rw-r--r--   0        0        0      548 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/__init__.py
+-rw-r--r--   0        0        0     8274 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/datasets_generation.py
+-rw-r--r--   0        0        0     7778 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/hierarchical_structure.py
+-rw-r--r--   0        0        0    62951 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/tsdataset.py
+-rw-r--r--   0        0        0    10283 2023-07-03 15:27:34.984775 etna-2.1.0/etna/datasets/utils.py
+-rw-r--r--   0        0        0      255 2023-07-03 15:27:34.984775 etna-2.1.0/etna/distributions/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-03 15:27:34.984775 etna-2.1.0/etna/distributions/distributions.py
+-rw-r--r--   0        0        0      226 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/__init__.py
+-rw-r--r--   0        0        0     6579 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/direct_ensemble.py
+-rw-r--r--   0        0        0     4684 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/mixins.py
+-rw-r--r--   0        0        0    11343 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/stacking_ensemble.py
+-rw-r--r--   0        0        0     9819 2023-07-03 15:27:34.984775 etna-2.1.0/etna/ensembles/voting_ensemble.py
+-rw-r--r--   0        0        0       94 2023-07-03 15:27:34.984775 etna-2.1.0/etna/experimental/change_points/__init__.py
+-rw-r--r--   0        0        0     5558 2023-07-03 15:27:34.984775 etna-2.1.0/etna/experimental/change_points/regularization_search.py
+-rw-r--r--   0        0        0      242 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/__init__.py
+-rw-r--r--   0        0        0      473 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/base.py
+-rw-r--r--   0        0        0     4926 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/classification.py
+-rw-r--r--   0        0        0      366 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/__init__.py
+-rw-r--r--   0        0        0     1543 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/base.py
+-rw-r--r--   0        0        0     2510 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/tsfresh.py
+-rw-r--r--   0        0        0    15250 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/feature_extraction/weasel.py
+-rw-r--r--   0        0        0     3241 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/predictability.py
+-rw-r--r--   0        0        0      874 2023-07-03 15:27:34.988775 etna-2.1.0/etna/experimental/classification/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pmdarima_utils/__init__.py
+-rw-r--r--   0        0        0     7455 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pmdarima_utils/arima.py
+-rw-r--r--   0        0        0      415 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pmdarima_utils/arima.pyi
+-rw-r--r--   0        0        0        0 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      472 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/pytorch_lightning/callbacks.py
+-rw-r--r--   0        0        0      341 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/__init__.py
+-rw-r--r--   0        0        0     1840 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/defaults.py
+-rw-r--r--   0        0        0     1801 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/distribution.py
+-rw-r--r--   0        0        0       69 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/distribution.pyi
+-rw-r--r--   0        0        0    16549 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/relevance.py
+-rw-r--r--   0        0        0      823 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/relevance.pyi
+-rw-r--r--   0        0        0     8470 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/significance_tests.py
+-rw-r--r--   0        0        0      344 2023-07-03 15:27:34.988775 etna-2.1.0/etna/libs/tsfresh/significance_tests.pyi
+-rw-r--r--   0        0        0      804 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/__init__.py
+-rw-r--r--   0        0        0     4993 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/base.py
+-rw-r--r--   0        0        0     2643 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/console_logger.py
+-rw-r--r--   0        0        0    15309 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/file_logger.py
+-rw-r--r--   0        0        0     7105 2023-07-03 15:27:34.988775 etna-2.1.0/etna/loggers/wandb_logger.py
+-rw-r--r--   0        0        0     1230 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/__init__.py
+-rw-r--r--   0        0        0     7625 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/base.py
+-rw-r--r--   0        0        0     5151 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/functional_metrics.py
+-rw-r--r--   0        0        0     5513 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/intervals_metrics.py
+-rw-r--r--   0        0        0     9643 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/metrics.py
+-rw-r--r--   0        0        0     2539 2023-07-03 15:27:34.988775 etna-2.1.0/etna/metrics/utils.py
+-rw-r--r--   0        0        0     1729 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/__init__.py
+-rw-r--r--   0        0        0     2521 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/autoarima.py
+-rw-r--r--   0        0        0    23070 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/base.py
+-rw-r--r--   0        0        0    16331 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/catboost.py
+-rw-r--r--   0        0        0    14394 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/deadline_ma.py
+-rw-r--r--   0        0        0      557 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/decorators.py
+-rw-r--r--   0        0        0    33314 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/holt_winters.py
+-rw-r--r--   0        0        0     8556 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/linear.py
+-rw-r--r--   0        0        0    22835 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/mixins.py
+-rw-r--r--   0        0        0      828 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/moving_average.py
+-rw-r--r--   0        0        0     1031 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/naive.py
+-rw-r--r--   0        0        0      373 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/__init__.py
+-rw-r--r--   0        0        0     9896 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepar.py
+-rw-r--r--   0        0        0      561 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/__init__.py
+-rw-r--r--   0        0        0    12488 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/deepstate.py
+-rw-r--r--   0        0        0     8808 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/linear_dynamic_system.py
+-rw-r--r--   0        0        0    12191 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/deepstate/state_space_model.py
+-rw-r--r--   0        0        0     9163 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/mlp.py
+-rw-r--r--   0        0        0    11237 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/rnn.py
+-rw-r--r--   0        0        0    11486 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/tft.py
+-rw-r--r--   0        0        0    12626 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/nn/utils.py
+-rw-r--r--   0        0        0    19903 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/prophet.py
+-rw-r--r--   0        0        0    33250 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/sarimax.py
+-rw-r--r--   0        0        0     8942 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/seasonal_ma.py
+-rw-r--r--   0        0        0     3555 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/sklearn.py
+-rw-r--r--   0        0        0    19716 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/tbats.py
+-rw-r--r--   0        0        0     3685 2023-07-03 15:27:34.988775 etna-2.1.0/etna/models/utils.py
+-rw-r--r--   0        0        0      292 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/__init__.py
+-rw-r--r--   0        0        0     5437 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/assembling_pipelines.py
+-rw-r--r--   0        0        0     7334 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/autoregressive_pipeline.py
+-rw-r--r--   0        0        0    39081 2023-07-03 15:27:34.988775 etna-2.1.0/etna/pipeline/base.py
+-rw-r--r--   0        0        0    14000 2023-07-03 15:27:34.992775 etna-2.1.0/etna/pipeline/hierarchical_pipeline.py
+-rw-r--r--   0        0        0     8460 2023-07-03 15:27:34.992775 etna-2.1.0/etna/pipeline/mixins.py
+-rw-r--r--   0        0        0     5563 2023-07-03 15:27:34.992775 etna-2.1.0/etna/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:27:34.992775 etna-2.1.0/etna/py.typed
+-rw-r--r--   0        0        0      181 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/__init__.py
+-rw-r--r--   0        0        0     3551 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/base.py
+-rw-r--r--   0        0        0     1899 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/bottom_up.py
+-rw-r--r--   0        0        0     5742 2023-07-03 15:27:34.992775 etna-2.1.0/etna/reconciliation/top_down.py
+-rw-r--r--   0        0        0    10540 2023-07-03 15:27:34.992775 etna-2.1.0/etna/settings.py
+-rw-r--r--   0        0        0     3286 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/__init__.py
+-rw-r--r--   0        0        0    12781 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/base.py
+-rw-r--r--   0        0        0     1168 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/__init__.py
+-rw-r--r--   0        0        0      949 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/__init__.py
+-rw-r--r--   0        0        0     7980 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/base.py
+-rw-r--r--   0        0        0      250 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
+-rw-r--r--   0        0        0     1886 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
+-rw-r--r--   0        0        0     2171 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
+-rw-r--r--   0        0        0     5666 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/detrend.py
+-rw-r--r--   0        0        0     5168 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/level.py
+-rw-r--r--   0        0        0      887 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
+-rw-r--r--   0        0        0      732 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
+-rw-r--r--   0        0        0     1311 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
+-rw-r--r--   0        0        0     3397 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
+-rw-r--r--   0        0        0     2496 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
+-rw-r--r--   0        0        0     5478 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/segmentation.py
+-rw-r--r--   0        0        0     5798 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/change_points_based/trend.py
+-rw-r--r--   0        0        0     8552 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/detrend.py
+-rw-r--r--   0        0        0     8239 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/decomposition/stl.py
+-rw-r--r--   0        0        0      306 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/__init__.py
+-rw-r--r--   0        0        0     7512 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/categorical.py
+-rw-r--r--   0        0        0     2836 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/mean_segment_encoder.py
+-rw-r--r--   0        0        0     2525 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/encoders/segment_encoder.py
+-rw-r--r--   0        0        0      444 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2469 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/base.py
+-rw-r--r--   0        0        0    10158 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/feature_importance.py
+-rw-r--r--   0        0        0     3434 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/filter.py
+-rw-r--r--   0        0        0    14975 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/feature_selection/gale_shapley.py
+-rw-r--r--   0        0        0     1383 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/__init__.py
+-rw-r--r--   0        0        0     4821 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/add_constant.py
+-rw-r--r--   0        0        0     5645 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/apply_lambda.py
+-rw-r--r--   0        0        0    17152 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/differencing.py
+-rw-r--r--   0        0        0     9987 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/lags.py
+-rw-r--r--   0        0        0     5002 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/log.py
+-rw-r--r--   0        0        0     4469 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/power.py
+-rw-r--r--   0        0        0    10377 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/scalers.py
+-rw-r--r--   0        0        0    11846 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/sklearn.py
+-rw-r--r--   0        0        0    22772 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/math/statistics.py
+-rw-r--r--   0        0        0      233 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/missing_values/__init__.py
+-rw-r--r--   0        0        0     9573 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/missing_values/imputation.py
+-rw-r--r--   0        0        0     6693 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/missing_values/resample.py
+-rw-r--r--   0        0        0      301 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/outliers/__init__.py
+-rw-r--r--   0        0        0     5106 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/outliers/base.py
+-rw-r--r--   0        0        0     7988 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/outliers/point_outliers.py
+-rw-r--r--   0        0        0      334 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/__init__.py
+-rw-r--r--   0        0        0    15747 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/date_flags.py
+-rw-r--r--   0        0        0     5802 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/fourier.py
+-rw-r--r--   0        0        0     2848 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/holiday.py
+-rw-r--r--   0        0        0     9079 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/special_days.py
+-rw-r--r--   0        0        0     9478 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/timestamp/time_flags.py
+-rw-r--r--   0        0        0      746 2023-07-03 15:27:34.992775 etna-2.1.0/etna/transforms/utils.py
+-rw-r--r--   0        0        0    11985 2023-07-03 15:27:35.228776 etna-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    19330 1970-01-01 00:00:00.000000 etna-2.1.0/PKG-INFO
```

### Comparing `etna-2.0.0/LICENSE` & `etna-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/README.md` & `etna-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -135,17 +135,19 @@
 ```bash
 pip install --upgrade pip
 pip install etna
 ```
 
 The default version doesn't contain all the dependencies, because some of them are needed only for specific models, e.g. Prophet, PyTorch.
 Available user extensions are the following:
-* `prophet`
-* `torch`
-* `wandb`
+* `prophet`: adds prophet model`,
+* `torch`: adds models based on neural nets,
+* `wandb`: adds wandb logger,
+* `auto`: adds AutoML functionality,
+* `classiciation`: adds time series classification functionality.
 
 Install extension:
 ```bash
 pip install etna[extension-name]
 ```
 
 Install all extensions:
@@ -185,40 +187,44 @@
 
 ## Documentation
 
 ETNA documentation is available [here](https://etna-docs.netlify.app/).
 
 ## Community
 
-To ask the questions or discuss the library you can join our [telegram chat](t.me/etna_support). 
+To ask the questions or discuss the library you can join our [telegram chat](https://t.me/etna_support). 
 [Discussions section](https://github.com/tinkoff-ai/etna/discussions) on github is also open for this purpose.
 
 ## Resources
 
 - [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium
 
 - [ETNA Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on Medium
 
 - [Time series forecasting with ETNA: first steps](https://medium.com/its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on Medium
 
 - [ETNA: Time Series Analysis. What, why and how?](https://medium.com/its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
 
+- [Time Series Forecasting Strategies in ETNA](https://medium.com/its-tinkoff/time-series-forecasting-strategies-in-etna-93d7d2f8a911) on Medium
+
 - [Tabular Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/code/chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on Kaggle
 
 - [Store sales prediction with etna library](https://www.kaggle.com/dmitrybunin/store-sales-prediction-with-etna-library?scriptVersionId=81104235) on Kaggle
 
 - [Tabular Playground Series - Jan 2022](https://www.kaggle.com/code/chikovalexander/tps-jan-2022-etna/notebook) on Kaggle
 
 - [EDA notebook for Ubiquant Market Prediction](https://www.kaggle.com/code/martins0n/ubiquant-eda-toy-predictions-etna) on Kaggle
 
 - [PyCon Russia September 2021 talk](https://youtu.be/VxWHLEFgXnE) on YouTube
 
 - [ETNA Meetup Jun 2022](https://www.youtube.com/watch?v=N1Xy3EqY058&list=PLLrf_044z4JrSsjMd-3dF6VbBLPI_yOxG) on YouTube
 
 - [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube
+
+- [Прикладные задачи анализа данных, лекция 8 — Временные ряды 2](https://youtu.be/1gXVbidDZck) on YouTube
  
 ## Acknowledgments
 
 ### ETNA.Team
 
 [Andrey Alekseev](https://github.com/iKintosh),
 [Nikita Barinov](https://github.com/diadorer),
@@ -228,15 +234,17 @@
 [Martin Gabdushev](https://github.com/martins0n),
 [Sergey Kolesnikov](https://github.com/Scitator),
 [Artem Makhin](https://github.com/Ama16),
 [Ivan Mitskovets](https://github.com/imitskovets),
 [Albina Munirova](https://github.com/albinamunirova),
 [Julia Shenshina](https://github.com/julia-shenshina),
 [Yuriy Tarasyuk](https://github.com/DBcreator),
-[Konstantin Vedernikov](https://github.com/scanhex12)
+[Konstantin Vedernikov](https://github.com/scanhex12),
+[Ivan Nedosekov](https://github.com/GrozniyToaster),
+[Rodion Petrov](https://github.com/Noidor1)
 
 ### ETNA.Contributors
 
 [WinstonDovlatov](https://github.com/WinstonDovlatov),
 [mvakhmenin](https://github.com/mvakhmenin),
 [Carlosbogo](https://github.com/Carlosbogo),
 [Pacman1984](https://github.com/Pacman1984),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -48,35 +48,38 @@
 y_pred=forecast_ts) >>> {'segment_b': 3.3017151519000967, 'segment_c':
 5.270557433427279, 'segment_a': 5.272811627335398, 'segment_d':
 4.689085450895735} ``` ## Installation ETNA is available on [PyPI](https://
 pypi.org/project/etna), so you can use `pip` to install it. Install default
 version: ```bash pip install --upgrade pip pip install etna ``` The default
 version doesn't contain all the dependencies, because some of them are needed
 only for specific models, e.g. Prophet, PyTorch. Available user extensions are
-the following: * `prophet` * `torch` * `wandb` Install extension: ```bash pip
-install etna[extension-name] ``` Install all extensions: ```bash pip install
-etna[all] ``` There are also developer extensions. All the extensions are
-listed in [`pyproject.toml`](https://github.com/tinkoff-ai/etna/blob/master/
-pyproject.toml#L93). Without the appropriate extension you will get an
-`ImportError` trying to import the model that needs it. For example,
-`etna.models.ProphetModel` needs `prophet` extension and can't be used without
-it. ### Configuration ETNA supports configuration files. It means that library
-will check that all the specified packages are installed prior to script start
-and NOT during runtime. To set up a configuration for your project you should
-create a `.etna` file at the project's root. To see the available options look
-at [`Settings`](https://github.com/tinkoff-ai/etna/blob/master/etna/
-settings.py#L68). There is an [example](https://github.com/tinkoff-ai/etna/
-tree/master/examples/configs/.etna) of configuration file. ## Tutorials We have
-also prepared a set of tutorials for an easy introduction: | Notebook |
-Interactive launch | |:----------|------:| | [Get started](https://github.com/
-tinkoff-ai/etna/tree/master/examples/get_started.ipynb) | [![Binder](https://
-mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
-master?filepath=examples/get_started.ipynb) | | [Backtest](https://github.com/
-tinkoff-ai/etna/tree/master/examples/backtest.ipynb) | [![Binder](https://
-mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
+the following: * `prophet`: adds prophet model`, * `torch`: adds models based
+on neural nets, * `wandb`: adds wandb logger, * `auto`: adds AutoML
+functionality, * `classiciation`: adds time series classification
+functionality. Install extension: ```bash pip install etna[extension-name] ```
+Install all extensions: ```bash pip install etna[all] ``` There are also
+developer extensions. All the extensions are listed in [`pyproject.toml`]
+(https://github.com/tinkoff-ai/etna/blob/master/pyproject.toml#L93). Without
+the appropriate extension you will get an `ImportError` trying to import the
+model that needs it. For example, `etna.models.ProphetModel` needs `prophet`
+extension and can't be used without it. ### Configuration ETNA supports
+configuration files. It means that library will check that all the specified
+packages are installed prior to script start and NOT during runtime. To set up
+a configuration for your project you should create a `.etna` file at the
+project's root. To see the available options look at [`Settings`](https://
+github.com/tinkoff-ai/etna/blob/master/etna/settings.py#L68). There is an
+[example](https://github.com/tinkoff-ai/etna/tree/master/examples/
+configs/.etna) of configuration file. ## Tutorials We have also prepared a set
+of tutorials for an easy introduction: | Notebook | Interactive launch | |:----
+------|------:| | [Get started](https://github.com/tinkoff-ai/etna/tree/master/
+examples/get_started.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)]
+(https://mybinder.org/v2/gh/tinkoff-ai/etna/master?filepath=examples/
+get_started.ipynb) | | [Backtest](https://github.com/tinkoff-ai/etna/tree/
+master/examples/backtest.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
 master?filepath=examples/backtest.ipynb) | | [EDA](https://github.com/tinkoff-
 ai/etna/tree/master/examples/EDA.ipynb) | [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
 master?filepath=examples/EDA.ipynb) | | [Outliers](https://github.com/tinkoff-
 ai/etna/tree/master/examples/outliers.ipynb) | [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
 master?filepath=examples/outliers.ipynb) | | [Clustering](https://github.com/
@@ -105,46 +108,52 @@
 tinkoff-ai/etna/master?filepath=examples/classification.ipynb) | |
 [Hierarchical time series](https://github.com/tinkoff-ai/etna/blob/master/
 examples/hierarchical_pipeline.ipynb) | [![Binder](https://mybinder.org/
 badge_logo.svg)](https://mybinder.org/v2/gh/tinkoff-ai/etna/
 master?filepath=examples/hierarchical_pipeline.ipynb) | ## Documentation ETNA
 documentation is available [here](https://etna-docs.netlify.app/). ## Community
 To ask the questions or discuss the library you can join our [telegram chat]
-(t.me/etna_support). [Discussions section](https://github.com/tinkoff-ai/etna/
-discussions) on github is also open for this purpose. ## Resources -
+(https://t.me/etna_support). [Discussions section](https://github.com/tinkoff-
+ai/etna/discussions) on github is also open for this purpose. ## Resources -
 [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/
 forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium - [ETNA
 Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on
 Medium - [Time series forecasting with ETNA: first steps](https://medium.com/
 its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on
 Medium - [ETNA: Time Series Analysis. What, why and how?](https://medium.com/
 its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
-- [Tabular Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/
-code/chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on
-Kaggle - [Store sales prediction with etna library](https://www.kaggle.com/
+- [Time Series Forecasting Strategies in ETNA](https://medium.com/its-tinkoff/
+time-series-forecasting-strategies-in-etna-93d7d2f8a911) on Medium - [Tabular
+Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/code/
+chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on Kaggle
+- [Store sales prediction with etna library](https://www.kaggle.com/
 dmitrybunin/store-sales-prediction-with-etna-library?scriptVersionId=81104235)
 on Kaggle - [Tabular Playground Series - Jan 2022](https://www.kaggle.com/code/
 chikovalexander/tps-jan-2022-etna/notebook) on Kaggle - [EDA notebook for
 Ubiquant Market Prediction](https://www.kaggle.com/code/martins0n/ubiquant-eda-
 toy-predictions-etna) on Kaggle - [PyCon Russia September 2021 talk](https://
 youtu.be/VxWHLEFgXnE) on YouTube - [ETNA Meetup Jun 2022](https://
 www.youtube.com/watch?v=N1Xy3EqY058&list=PLLrf_044z4JrSsjMd-3dF6VbBLPI_yOxG) on
-YouTube - [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube ##
+YouTube - [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube -
+[ÐÑÐ¸ÐºÐ»Ð°Ð´Ð½ÑÐµ Ð·Ð°Ð´Ð°ÑÐ¸ Ð°Ð½Ð°Ð»Ð¸Ð·Ð° Ð´Ð°Ð½Ð½ÑÑ, Ð»ÐµÐºÑÐ¸Ñ 8
+â ÐÑÐµÐ¼ÐµÐ½Ð½ÑÐµ ÑÑÐ´Ñ 2](https://youtu.be/1gXVbidDZck) on YouTube ##
 Acknowledgments ### ETNA.Team [Andrey Alekseev](https://github.com/iKintosh),
 [Nikita Barinov](https://github.com/diadorer), [Dmitriy Bunin](https://
 github.com/Mr-Geekman), [Aleksandr Chikov](https://github.com/alex-hse-
 repository), [Vladislav Denisov](https://github.com/v-v-denisov), [Martin
 Gabdushev](https://github.com/martins0n), [Sergey Kolesnikov](https://
 github.com/Scitator), [Artem Makhin](https://github.com/Ama16), [Ivan
 Mitskovets](https://github.com/imitskovets), [Albina Munirova](https://
 github.com/albinamunirova), [Julia Shenshina](https://github.com/julia-
 shenshina), [Yuriy Tarasyuk](https://github.com/DBcreator), [Konstantin
-Vedernikov](https://github.com/scanhex12) ### ETNA.Contributors
-[WinstonDovlatov](https://github.com/WinstonDovlatov), [mvakhmenin](https://
-github.com/mvakhmenin), [Carlosbogo](https://github.com/Carlosbogo),
-[Pacman1984](https://github.com/Pacman1984), [looopka](https://github.com/
-looopka), [Artem Levashov](https://github.com/soft1q), [Aleksey Podkidyshev]
-(https://github.com/alekseyen) ## License Feel free to use our library in your
-commercial and private applications. ETNA is covered by [Apache 2.0](/LICENSE).
-Read more about this license [here](https://choosealicense.com/licenses/apache-
-2.0/) > Please note that `etna[prophet]` is covered by [GPL 2.0](https://
-www.gnu.org/licenses/old-licenses/gpl-2.0.html) due to pystan package.
+Vedernikov](https://github.com/scanhex12), [Ivan Nedosekov](https://github.com/
+GrozniyToaster), [Rodion Petrov](https://github.com/Noidor1) ###
+ETNA.Contributors [WinstonDovlatov](https://github.com/WinstonDovlatov),
+[mvakhmenin](https://github.com/mvakhmenin), [Carlosbogo](https://github.com/
+Carlosbogo), [Pacman1984](https://github.com/Pacman1984), [looopka](https://
+github.com/looopka), [Artem Levashov](https://github.com/soft1q), [Aleksey
+Podkidyshev](https://github.com/alekseyen) ## License Feel free to use our
+library in your commercial and private applications. ETNA is covered by [Apache
+2.0](/LICENSE). Read more about this license [here](https://choosealicense.com/
+licenses/apache-2.0/) > Please note that `etna[prophet]` is covered by [GPL
+2.0](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html) due to pystan
+package.
```

### Comparing `etna-2.0.0/etna/analysis/__init__.py` & `etna-2.1.0/etna/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/decomposition/__init__.py` & `etna-2.1.0/etna/analysis/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/decomposition/plots.py` & `etna-2.1.0/etna/analysis/decomposition/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/decomposition/search.py` & `etna-2.1.0/etna/analysis/decomposition/search.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/decomposition/utils.py` & `etna-2.1.0/etna/analysis/decomposition/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/eda/plots.py` & `etna-2.1.0/etna/analysis/eda/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/eda/utils.py` & `etna-2.1.0/etna/analysis/eda/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,17 @@
     timestamp = index.tolist()
     country_holidays = holidays_lib.country_holidays(country=holidays)
     holiday_names = {country_holidays.get(timestamp_value) for timestamp_value in timestamp}
     holiday_names = holiday_names.difference({None})
 
     holidays_dict = {}
     for holiday_name in holiday_names:
-        cur_holiday_index = pd.Series(timestamp).apply(lambda x: country_holidays.get(x, "") == holiday_name)
+        cur_holiday_index = pd.Series(timestamp).apply(
+            lambda x: country_holidays.get(x, "") == holiday_name  # noqa: B023
+        )
         holidays_dict[holiday_name] = cur_holiday_index
 
     holidays_df = pd.DataFrame(holidays_dict)
     holidays_df.index = timestamp
     return holidays_df
```

### Comparing `etna-2.0.0/etna/analysis/feature_relevance/plots.py` & `etna-2.1.0/etna/analysis/feature_relevance/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/feature_relevance/relevance.py` & `etna-2.1.0/etna/analysis/feature_relevance/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/feature_relevance/relevance_table.py` & `etna-2.1.0/etna/analysis/feature_relevance/relevance_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,29 @@
     if len(common_index) < len(df.loc[first_valid_idx:, segment]):
         warnings.warn("Exogenous or target data contains None! It will be dropped for calculating relevance.")
     return df_seg.loc[common_index], df_exog_seg.loc[common_index]
 
 
 def get_statistics_relevance_table(df: pd.DataFrame, df_exog: pd.DataFrame) -> pd.DataFrame:
     """Calculate relevance table with p-values from tsfresh.
-
     Parameters
     ----------
     df:
         dataframe with timeseries
     df_exog:
         dataframe with exogenous data
 
     Returns
     -------
     pd.DataFrame
         dataframe with p-values.
+
+    Notes
+    -----
+    Time complexity of this method is :math:`O(n\_segments * n\_features * history\_len)`
     """
     regressors = sorted(df_exog.columns.get_level_values("feature").unique())
     segments = sorted(df.columns.get_level_values("segment").unique())
     result = np.empty((len(segments), len(regressors)))
     for k, seg in enumerate(segments):
         df_seg, df_exog_seg = _prepare_df(df=df, df_exog=df_exog, segment=seg, regressors=regressors)
         cat_cols = df_exog_seg.dtypes[df_exog_seg.dtypes == "category"].index
@@ -60,15 +63,17 @@
                 df_exog_seg[cat_col] = df_exog_seg[cat_col].astype(float)
             except ValueError:
                 raise ValueError(f"{cat_col} column cannot be cast to float type! Please, use encoders.")
             warnings.warn(
                 "Exogenous data contains columns with category type! It will be converted to float. If this is not desired behavior, use encoders."
             )
 
-        relevance = calculate_relevance_table(X=df_exog_seg, y=df_seg)[["feature", "p_value"]].values
+        relevance = calculate_relevance_table(X=df_exog_seg, y=df_seg, ml_task="regression")[
+            ["feature", "p_value"]
+        ].values
         result[k] = np.array(sorted(relevance, key=lambda x: x[0]))[:, 1]
     relevance_table = pd.DataFrame(result)
     relevance_table.index = segments
     relevance_table.columns = regressors
     return relevance_table
```

### Comparing `etna-2.0.0/etna/analysis/feature_relevance/utils.py` & `etna-2.1.0/etna/analysis/feature_relevance/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/feature_selection/mrmr_selection.py` & `etna-2.1.0/etna/analysis/feature_selection/mrmr_selection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from enum import Enum
 from typing import List
 
 import numpy as np
 import pandas as pd
 
 
@@ -22,14 +23,15 @@
 }
 
 
 def mrmr(
     relevance_table: pd.DataFrame,
     regressors: pd.DataFrame,
     top_k: int,
+    fast_redundancy: bool = False,
     relevance_aggregation_mode: str = AggregationMode.mean,
     redundancy_aggregation_mode: str = AggregationMode.mean,
     atol: float = 1e-10,
 ) -> List[str]:
     """
     Maximum Relevance and Minimum Redundancy feature selection method.
 
@@ -43,53 +45,75 @@
     relevance_table:
         dataframe of shape n_segment x n_exog_series with relevance table, where ``relevance_table[i][j]``
         contains relevance of j-th ``df_exog`` series to i-th df series
     regressors:
         dataframe with regressors in etna format
     top_k:
         num of regressors to select; if there are not enough regressors, then all will be selected
+    fast_redundancy:
+        * True: compute redundancy only inside the the segments, time complexity :math:`O(top\_k * n\_segments * n\_features * history\_len)`
+        * False: compute redundancy for all the pairs of segments, time complexity :math:`O(top\_k * n\_segments^2 * n\_features * history\_len)`
     relevance_aggregation_mode:
         the method for relevance values per-segment aggregation
     redundancy_aggregation_mode:
         the method for redundancy values per-segment aggregation
     atol:
         the absolute tolerance to compare the float values
 
     Returns
     -------
     selected_features: List[str]
         list of ``top_k`` selected regressors, sorted by their importance
     """
+    if not fast_redundancy:
+        warnings.warn(
+            "Option `fast_redundancy=False` was added for backward compatibility and will be removed in etna 3.0.0.",
+            DeprecationWarning,
+        )
     relevance_aggregation_fn = AGGREGATION_FN[AggregationMode(relevance_aggregation_mode)]
     redundancy_aggregation_fn = AGGREGATION_FN[AggregationMode(redundancy_aggregation_mode)]
 
     relevance = relevance_table.apply(relevance_aggregation_fn).fillna(0)
 
     all_features = relevance.index.to_list()
+    segments = set(regressors.columns.get_level_values("segment"))
     selected_features: List[str] = []
     not_selected_features = all_features.copy()
 
     redundancy_table = pd.DataFrame(np.inf, index=all_features, columns=all_features)
     top_k = min(top_k, len(all_features))
 
     for i in range(top_k):
         score_numerator = relevance.loc[not_selected_features]
         score_denominator = pd.Series(1, index=not_selected_features)
         if i > 0:
             last_selected_feature = selected_features[-1]
-            not_selected_regressors = regressors.loc[pd.IndexSlice[:], pd.IndexSlice[:, not_selected_features]]
             last_selected_regressor = regressors.loc[pd.IndexSlice[:], pd.IndexSlice[:, last_selected_feature]]
+            not_selected_regressors = regressors.loc[pd.IndexSlice[:], pd.IndexSlice[:, not_selected_features]]
+
+            if fast_redundancy:
+                segment_redundancy = pd.concat(
+                    [
+                        not_selected_regressors[segment].apply(
+                            lambda col: last_selected_regressor[segment].corrwith(col)  # noqa: B023
+                        )
+                        for segment in segments
+                    ]
+                ).abs()
+            else:
+                segment_redundancy = (
+                    not_selected_regressors.apply(lambda col: last_selected_regressor.corrwith(col))  # noqa: B023
+                    .abs()
+                    .groupby("feature")
+                    .apply(redundancy_aggregation_fn)
+                    .T.groupby("feature")
+                )
 
             redundancy_table.loc[not_selected_features, last_selected_feature] = (
-                not_selected_regressors.apply(lambda col: last_selected_regressor.corrwith(col))
-                .abs()
-                .groupby("feature")
-                .apply(redundancy_aggregation_fn)
-                .T.groupby("feature")
-                .apply(redundancy_aggregation_fn)
+                segment_redundancy.apply(redundancy_aggregation_fn)
                 .clip(atol)
                 .fillna(np.inf)
                 .loc[not_selected_features]
                 .values.squeeze()
             )
 
             score_denominator = redundancy_table.loc[not_selected_features, selected_features].mean(axis=1)
```

### Comparing `etna-2.0.0/etna/analysis/forecast/__init__.py` & `etna-2.1.0/etna/analysis/forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/forecast/plots.py` & `etna-2.1.0/etna/analysis/forecast/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,47 +240,48 @@
     folds = sorted(set(fold_numbers))
 
     # prepare dataframes
     df = ts.df
     forecast_start = forecast_df.index.min()
     history_df = df[df.index < forecast_start]
     backtest_df = df[df.index >= forecast_start]
-    freq_timedelta = df.index[1] - df.index[0]
 
     # prepare colors
     default_colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
     color_cycle = itertools.cycle(default_colors)
     lines_colors = {line_name: next(color_cycle) for line_name in ["history", "test", "forecast"]}
 
     _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
     for i, segment in enumerate(segments):
         segment_backtest_df = backtest_df[segment]
         segment_history_df = history_df[segment]
         segment_forecast_df = forecast_df[segment]
         is_full_folds = set(segment_backtest_df.index) == set(segment_forecast_df.index)
+        single_point_forecast = len(segment_backtest_df) == 1
+        draw_only_lines = is_full_folds and not single_point_forecast
 
         # plot history
         if history_len == "all":
             plot_df = pd.concat((segment_history_df, segment_backtest_df))
         elif history_len > 0:
             plot_df = pd.concat((segment_history_df.tail(history_len), segment_backtest_df))
         else:
             plot_df = segment_backtest_df
         ax[i].plot(plot_df.index, plot_df.target, color=lines_colors["history"])
 
         for fold_number in folds:
             start_fold = fold_numbers[fold_numbers == fold_number].index.min()
             end_fold = fold_numbers[fold_numbers == fold_number].index.max()
-            end_fold_exclusive = end_fold + freq_timedelta
+            end_fold_exclusive = pd.date_range(start=end_fold, periods=2, freq=ts.freq)[1]
 
             # draw test
             backtest_df_slice_fold = segment_backtest_df[start_fold:end_fold_exclusive]
             ax[i].plot(backtest_df_slice_fold.index, backtest_df_slice_fold.target, color=lines_colors["test"])
 
-            if is_full_folds:
+            if draw_only_lines:
                 # draw forecast
                 forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold_exclusive]
                 ax[i].plot(forecast_df_slice_fold.index, forecast_df_slice_fold.target, color=lines_colors["forecast"])
             else:
                 forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold]
                 backtest_df_slice_fold = backtest_df_slice_fold.loc[forecast_df_slice_fold.index]
 
@@ -356,25 +357,26 @@
     folds = sorted(set(fold_numbers))
 
     # prepare dataframes
     df = ts.df
     forecast_start = forecast_df.index.min()
     history_df = df[df.index < forecast_start]
     backtest_df = df[df.index >= forecast_start]
-    freq_timedelta = df.index[1] - df.index[0]
 
     # prepare colors
     colors = plotly.colors.qualitative.Dark24
 
     fig = go.Figure()
     for i, segment in enumerate(segments):
         segment_backtest_df = backtest_df[segment]
         segment_history_df = history_df[segment]
         segment_forecast_df = forecast_df[segment]
         is_full_folds = set(segment_backtest_df.index) == set(segment_forecast_df.index)
+        single_point_forecast = len(segment_backtest_df) == 1
+        draw_only_lines = is_full_folds and not single_point_forecast
 
         # plot history
         if history_len == "all":
             plot_df = segment_history_df.append(segment_backtest_df)
         elif history_len > 0:
             plot_df = segment_history_df.tail(history_len).append(segment_backtest_df)
         else:
@@ -391,15 +393,15 @@
                 line=dict(width=2, dash="dash"),
             )
         )
 
         for fold_number in folds:
             start_fold = fold_numbers[fold_numbers == fold_number].index.min()
             end_fold = fold_numbers[fold_numbers == fold_number].index.max()
-            end_fold_exclusive = end_fold + freq_timedelta
+            end_fold_exclusive = pd.date_range(start=end_fold, periods=2, freq=ts.freq)[1]
 
             # draw test
             backtest_df_slice_fold = segment_backtest_df[start_fold:end_fold_exclusive]
             fig.add_trace(
                 go.Scattergl(
                     x=backtest_df_slice_fold.index,
                     y=backtest_df_slice_fold.target,
@@ -408,15 +410,15 @@
                     mode="lines",
                     marker_color=colors[i % len(colors)],
                     showlegend=False,
                     line=dict(width=2, dash="solid"),
                 )
             )
 
-            if is_full_folds:
+            if draw_only_lines:
                 # draw forecast
                 forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold_exclusive]
                 fig.add_trace(
                     go.Scattergl(
                         x=forecast_df_slice_fold.index,
                         y=forecast_df_slice_fold.target,
                         legendgroup=f"{segment}",
```

### Comparing `etna-2.0.0/etna/analysis/forecast/utils.py` & `etna-2.1.0/etna/analysis/forecast/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import warnings
+from copy import deepcopy
 from typing import TYPE_CHECKING
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Union
 
@@ -11,48 +12,51 @@
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 def get_residuals(forecast_df: pd.DataFrame, ts: "TSDataset") -> "TSDataset":
     """Get residuals for further analysis.
 
+    Function keeps hierarchy, features in result dataset and removes target components.
+
     Parameters
     ----------
     forecast_df:
         forecasted dataframe with timeseries data
     ts:
         dataset of timeseries that has answers to forecast
 
     Returns
     -------
-    new_ts: TSDataset
+    new_ts:
         TSDataset with residuals in forecasts
 
     Raises
     ------
     KeyError:
         if segments of ``forecast_df`` and ``ts`` aren't the same
-
-    Notes
-    -----
-    Transforms are taken as is from ``ts``.
     """
     from etna.datasets import TSDataset
 
+    # remove target components
+    ts_copy = deepcopy(ts)
+    ts_copy.drop_target_components()
+
     # find the residuals
-    true_df = ts[forecast_df.index, :, :]
-    if set(ts.segments) != set(forecast_df.columns.get_level_values("segment").unique()):
+    true_df = ts_copy[forecast_df.index, :, :]
+    if set(ts_copy.segments) != set(forecast_df.columns.get_level_values("segment").unique()):
         raise KeyError("Segments of `ts` and `forecast_df` should be the same")
     true_df.loc[:, pd.IndexSlice[ts.segments, "target"]] -= forecast_df.loc[:, pd.IndexSlice[ts.segments, "target"]]
 
     # make TSDataset
-    new_ts = TSDataset(df=true_df, freq=ts.freq)
-    new_ts.known_future = ts.known_future
-    new_ts._regressors = ts.regressors
-    new_ts.df_exog = ts.df_exog
+    new_ts = TSDataset(df=true_df, freq=ts_copy.freq, hierarchical_structure=ts_copy.hierarchical_structure)
+    new_ts.known_future = deepcopy(ts_copy.known_future)
+    new_ts._regressors = deepcopy(ts_copy.regressors)
+    if ts.df_exog is not None:
+        new_ts.df_exog = ts.df_exog.copy(deep=True)
     return new_ts
 
 
 def _get_existing_quantiles(ts: "TSDataset") -> Set[float]:
     """Get quantiles that are present inside the TSDataset."""
     cols = [col for col in ts.columns.get_level_values("feature").unique().tolist() if col.startswith("target_0.")]
     existing_quantiles = {float(col[len("target_") :]) for col in cols}
```

### Comparing `etna-2.0.0/etna/analysis/outliers/__init__.py` & `etna-2.1.0/etna/analysis/outliers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/outliers/density_outliers.py` & `etna-2.1.0/etna/analysis/outliers/density_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/outliers/hist_outliers.py` & `etna-2.1.0/etna/analysis/outliers/hist_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/outliers/median_outliers.py` & `etna-2.1.0/etna/analysis/outliers/median_outliers.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/outliers/plots.py` & `etna-2.1.0/etna/analysis/outliers/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/analysis/outliers/prediction_interval_outliers.py` & `etna-2.1.0/etna/analysis/outliers/prediction_interval_outliers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,72 @@
 from copy import deepcopy
 from typing import TYPE_CHECKING
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import Union
 
-import numpy as np
 import pandas as pd
 
+from etna.datasets import TSDataset
+
 if TYPE_CHECKING:
-    from etna.datasets import TSDataset
     from etna.models import ProphetModel
     from etna.models import SARIMAXModel
 
 
-def create_ts_by_column(ts: "TSDataset", column: str) -> "TSDataset":
+def create_ts_by_column(ts: TSDataset, column: str) -> TSDataset:
     """Create TSDataset based on original ts with selecting only column in each segment and setting it to target.
 
     Parameters
     ----------
     ts:
         dataset with timeseries data
     column:
         column to select in each.
 
     Returns
     -------
     result: TSDataset
         dataset with selected column.
     """
-    from etna.datasets import TSDataset
-
     new_df = ts[:, :, [column]]
     new_columns_tuples = [(x[0], "target") for x in new_df.columns.tolist()]
     new_df.columns = pd.MultiIndex.from_tuples(new_columns_tuples, names=new_df.columns.names)
     return TSDataset(new_df, freq=ts.freq)
 
 
+def _select_segments_subset(ts: TSDataset, segments: List[str]) -> TSDataset:
+    """Create TSDataset with certain segments.
+
+    Parameters
+    ----------
+    ts:
+        dataset with timeseries data
+    segments:
+        list with segments names
+
+    Returns
+    -------
+    result: TSDataset
+        dataset with selected column.
+    """
+    df = ts.raw_df.loc[:, pd.IndexSlice[segments, :]].copy()
+    df = df.dropna()
+    df_exog = ts.df_exog
+    if df_exog is not None:
+        df_exog = df_exog.loc[df.index, pd.IndexSlice[segments, :]].copy()
+    known_future = ts.known_future
+    freq = ts.freq
+    subset_ts = TSDataset(df=df, df_exog=df_exog, known_future=known_future, freq=freq)
+    return subset_ts
+
+
 def get_anomalies_prediction_interval(
-    ts: "TSDataset",
+    ts: TSDataset,
     model: Union[Type["ProphetModel"], Type["SARIMAXModel"]],
     interval_width: float = 0.95,
     in_column: str = "target",
     **model_params,
 ) -> Dict[str, List[pd.Timestamp]]:
     """
     Get point outliers in time series using prediction intervals (estimation model-based method).
@@ -74,22 +98,22 @@
     For not "target" column only column data will be used for learning.
     """
     if in_column == "target":
         ts_inner = ts
     else:
         ts_inner = create_ts_by_column(ts, in_column)
     outliers_per_segment = {}
-    time_points = np.array(ts.index.values)
     model_instance = model(**model_params)
     model_instance.fit(ts_inner)
     lower_p, upper_p = [(1 - interval_width) / 2, (1 + interval_width) / 2]
-    prediction_interval = model_instance.predict(
-        deepcopy(ts_inner), prediction_interval=True, quantiles=[lower_p, upper_p]
-    )
     for segment in ts_inner.segments:
-        predicted_segment_slice = prediction_interval[:, segment, :][segment]
-        actual_segment_slice = ts_inner[:, segment, :][segment]
+        ts_segment = _select_segments_subset(ts=ts_inner, segments=[segment])
+        prediction_interval = model_instance.predict(
+            deepcopy(ts_segment), prediction_interval=True, quantiles=[lower_p, upper_p]
+        )
+        actual_segment_slice = ts_segment[:, segment, :][segment]
+        predicted_segment_slice = prediction_interval[actual_segment_slice.index, segment, :][segment]
         anomalies_mask = (actual_segment_slice["target"] > predicted_segment_slice[f"target_{upper_p:.4g}"]) | (
             actual_segment_slice["target"] < predicted_segment_slice[f"target_{lower_p:.4g}"]
         )
-        outliers_per_segment[segment] = list(time_points[anomalies_mask])
+        outliers_per_segment[segment] = list(predicted_segment_slice[anomalies_mask].index.values)
     return outliers_per_segment
```

### Comparing `etna-2.0.0/etna/analysis/utils.py` & `etna-2.1.0/etna/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/auto/optuna/config_sampler.py` & `etna-2.1.0/etna/auto/optuna/config_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partial
 from typing import List
 from typing import Optional
 from typing import Set
 
 import numpy as np
 from optuna.samplers import BaseSampler
 from optuna.study import Study
@@ -111,18 +112,18 @@
         running_trials_hash = []
 
         for t in trials:
             if t.state.is_finished():
                 finished_trials_hash.append(t.user_attrs["hash"])
             elif t.state == TrialState.RUNNING:
 
-                def _closure():
-                    return study._storage.get_trial(t._trial_id).user_attrs["hash"]
+                def _closure(trial):
+                    return study._storage.get_trial(trial._trial_id).user_attrs["hash"]
 
-                hash_to_add = retry(_closure, max_retries=self.retries)
+                hash_to_add = retry(partial(_closure, trial=t), max_retries=self.retries)
                 running_trials_hash.append(hash_to_add)
             else:
                 pass
 
         return set(self.configs_hash) - set(finished_trials_hash) - set(running_trials_hash)
 
     @property
```

### Comparing `etna-2.0.0/etna/auto/optuna/wrapper.py` & `etna-2.1.0/etna/auto/optuna/wrapper.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/auto/pool/generator.py` & `etna-2.1.0/etna/auto/pool/generator.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/auto/pool/templates.py` & `etna-2.1.0/etna/auto/pool/templates.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/auto/runner/local.py` & `etna-2.1.0/etna/auto/runner/local.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/__init__.py` & `etna-2.1.0/etna/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/base.py` & `etna-2.1.0/etna/clustering/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/distances/base.py` & `etna-2.1.0/etna/clustering/distances/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/distances/distance_matrix.py` & `etna-2.1.0/etna/clustering/distances/distance_matrix.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/distances/dtw_distance.py` & `etna-2.1.0/etna/clustering/distances/dtw_distance.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/distances/euclidean_distance.py` & `etna-2.1.0/etna/clustering/distances/euclidean_distance.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/hierarchical/base.py` & `etna-2.1.0/etna/clustering/hierarchical/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from etna.clustering.base import Clustering
 from etna.clustering.distances.base import Distance
 from etna.clustering.distances.distance_matrix import DistanceMatrix
 from etna.datasets import TSDataset
 
 
-class ClusteringLinkageMode(Enum):
+class ClusteringLinkageMode(str, Enum):
     """Modes allowed for clustering distance computation."""
 
     ward = "ward"
     complete = "complete"
     average = "average"
     single = "single"
```

### Comparing `etna-2.0.0/etna/clustering/hierarchical/dtw_clustering.py` & `etna-2.1.0/etna/clustering/hierarchical/dtw_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/clustering/hierarchical/euclidean_clustering.py` & `etna-2.1.0/etna/clustering/hierarchical/euclidean_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/core/mixins.py` & `etna-2.1.0/etna/core/mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import inspect
 import json
 import pathlib
-import pickle
 import sys
 import warnings
 import zipfile
 from enum import Enum
 from typing import Any
 from typing import Callable
 from typing import Dict
-from typing import List
+from typing import Sequence
 from typing import Tuple
+from typing import TypeVar
 from typing import cast
 
+import dill
 import hydra_slayer
 from sklearn.base import BaseEstimator
+from typing_extensions import Self
+
+from etna.core.saving import AbstractSaveable
+
+TMixin = TypeVar("TMixin", bound="BaseMixin")
 
 
 class BaseMixin:
     """Base mixin for etna classes."""
 
     def __repr__(self):
         """Get default representation of etna object."""
@@ -56,23 +62,24 @@
             return value.to_dict()
         elif isinstance(value, BaseEstimator):
             answer = {}
             answer["_target_"] = BaseMixin._get_target_from_class(value)
             model_parameters = value.get_params()
             answer.update(model_parameters)
             return answer
+        # this if is for objects imported from etna.libs.pytorch_lightning.callbacks
         elif hasattr(value, "_init_params"):
             return {"_target_": BaseMixin._get_target_from_class(value), **value._init_params}
         elif isinstance(value, (str, float, int)):
             return value
-        elif isinstance(value, List):
+        elif isinstance(value, list):
             return [BaseMixin._parse_value(elem) for elem in value]
         elif isinstance(value, tuple):
             return tuple([BaseMixin._parse_value(elem) for elem in value])
-        elif isinstance(value, Dict):
+        elif isinstance(value, dict):
             return {key: BaseMixin._parse_value(item) for key, item in value.items()}
         elif inspect.isfunction(value):
             return {"_target_": BaseMixin._get_target_from_function(value)}
         else:
             answer = {}
             answer["_target_"] = BaseMixin._get_target_from_class(value)
             warnings.warn("Some of external objects in input parameters could be not written in dict")
@@ -86,57 +93,95 @@
             value = self.__dict__[arg]
             if value is None:
                 continue
             params[arg] = BaseMixin._parse_value(value=value)
         params["_target_"] = BaseMixin._get_target_from_class(self)
         return params
 
-    @staticmethod
-    def _update_nested_dict_with_flat_dict(params_dict: dict, flat_dict: dict):
-        """Update nested dict with flat dict.
+    @classmethod
+    def _update_nested_structure(cls, structure: Any, keys: Sequence[str], value: Any) -> Any:
+        """Update nested structure by sequence of keys with value.
 
-        The method updates ``params_dict`` with values from ``flat_dict``,
-        so that ``params_dict`` contains all the nested keys of two given dicts,
-        e.g. for ``params_dict = {"model": {"learning_rate": value1}}``
-        and ``flat_dict = {"model.depth": value2}``
-        resulting ``params_dict`` will be
-        ``{"model": {"depth": value1, "learning_rate": value2}}``
+        Method applies sequence of keys to structure and returns the structure with changed value.
+        Key can only be applied to ``dict``, ``list`` or ``tuple``.
+        For ``list`` and ``tuple`` function ``int`` is used to make index from the key.
+
+        Raises
+        ------
+        ValueError:
+            Unsupported type of structure to update
+        """
+        if len(keys) == 0:
+            return value
 
-        Parameters
-        ----------
-        **params_dict: dict
-            dict with nested parameters structure, e.g ``{"model": {"learning_rate": value1}}``
-        **flat_dict: dict
-            dict with flat paratemers structure, e.g. ``{"model.depth": value2}``
+        current_key = keys[0]
+        new_structure: Any
+        if isinstance(structure, dict):
+            structure_to_update = structure.get(current_key, {})
+            current_value = cls._update_nested_structure(structure_to_update, keys[1:], value)
+            new_structure = structure
+            new_structure[current_key] = current_value
+        elif isinstance(structure, list):
+            idx = int(current_key)
+            structure_to_update = structure[idx]
+            current_value = cls._update_nested_structure(structure_to_update, keys[1:], value)
+            new_structure = structure
+            new_structure[idx] = current_value
+        elif isinstance(structure, tuple):
+            idx = int(current_key)
+            structure_to_update = structure[idx]
+            current_value = cls._update_nested_structure(structure_to_update, keys[1:], value)
+            new_temp_structure = list(structure)
+            new_temp_structure[idx] = current_value
+            new_structure = tuple(new_temp_structure)
+        else:
+            raise ValueError(
+                f"Structure to update is {structure} with type {type(structure)}, allowed types are dict, list, tuple"
+            )
 
-        """
-        for param, param_value in flat_dict.items():
-            *param_nesting, param_attr = param.split(".")
-            cycle_dict = params_dict
-            for param_nested in param_nesting:
-                cycle_dict = cycle_dict.setdefault(param_nested, {})
-            cycle_dict[param_attr] = param_value
+        return new_structure
 
-    def set_params(self, **params: dict) -> "BaseMixin":
+    def set_params(self: TMixin, **params: dict) -> TMixin:
         """Return new object instance with modified parameters.
 
-        The method works on simple estimators as well as on nested objects
-        (such as :class:`~etna.pipeline.Pipeline`). The latter have
-        parameters of the form ``<component>.<parameter>`` so that it's
-        possible to update each component of a nested object.
+        Method also allows to change parameters of nested objects within the current object.
+        For example, it is possible to change parameters of a ``model`` in a :class:`~etna.pipeline.Pipeline`.
+
+        Nested parameters are expected to be in a ``<component_1>.<...>.<parameter>`` form,
+        where components are separated by a dot.
 
         Parameters
         ----------
-        **params: dict
-            Estimator parameters.
+        **params:
+            Estimator parameters
 
+        Returns
+        -------
+        :
+            New instance with changed parameters
+
+        Examples
+        --------
+        >>> from etna.pipeline import Pipeline
+        >>> from etna.models import NaiveModel
+        >>> from etna.transforms import AddConstTransform
+        >>> model = model=NaiveModel(lag=1)
+        >>> transforms = [AddConstTransform(in_column="target", value=1)]
+        >>> pipeline = Pipeline(model, transforms=transforms, horizon=3)
+        >>> pipeline.set_params(**{"model.lag": 3, "transforms.0.value": 2})
+        Pipeline(model = NaiveModel(lag = 3, ), transforms = [AddConstTransform(in_column = 'target', value = 2, inplace = True, out_column = None, )], horizon = 3, )
         """
         params_dict = self.to_dict()
-        self._update_nested_dict_with_flat_dict(params_dict, params)
-        estimator_out = hydra_slayer.get_from_params(**params_dict)
+
+        new_params_dict = params_dict
+        for current_key, value in params.items():
+            keys = current_key.split(".")
+            new_params_dict = self._update_nested_structure(new_params_dict, keys, value)
+
+        estimator_out = hydra_slayer.get_from_params(**new_params_dict)
         return estimator_out
 
 
 class StringEnumWithRepr(str, Enum):
     """Base class for str enums, that has alternative __repr__ method."""
 
     def __repr__(self):
@@ -159,15 +204,15 @@
 
         str_version = pkg_resources.get_distribution("etna").version
         result = tuple([int(x) for x in str_version.split(".")])
         result = cast(Tuple[int, int, int], result)
         return result
 
 
-class SaveMixin:
+class SaveMixin(AbstractSaveable):
     """Basic implementation of ``AbstractSaveable`` abstract class.
 
     It saves object to the zip archive with 2 files:
 
     * metadata.json: contains library version and class name.
 
     * object.pkl: pickled object.
@@ -182,15 +227,15 @@
         metadata_str = json.dumps(metadata, indent=2, sort_keys=True)
         metadata_bytes = metadata_str.encode("utf-8")
         with archive.open("metadata.json", "w") as output_file:
             output_file.write(metadata_bytes)
 
     def _save_state(self, archive: zipfile.ZipFile):
         with archive.open("object.pkl", "w") as output_file:
-            pickle.dump(self, output_file)
+            dill.dump(self, output_file)
 
     def save(self, path: pathlib.Path):
         """Save the object.
 
         Parameters
         ----------
         path:
@@ -219,20 +264,20 @@
             saved_etna_version_str = ".".join([str(x) for x in saved_etna_version])
             warnings.warn(
                 f"The object was saved under etna version {saved_etna_version_str} "
                 f"but running version is {current_etna_version_str}, this can cause problems with compatibility!"
             )
 
     @classmethod
-    def _load_state(cls, archive: zipfile.ZipFile) -> Any:
+    def _load_state(cls, archive: zipfile.ZipFile) -> Self:
         with archive.open("object.pkl", "r") as input_file:
-            return pickle.load(input_file)
+            return dill.load(input_file)
 
     @classmethod
-    def load(cls, path: pathlib.Path) -> Any:
+    def load(cls, path: pathlib.Path) -> Self:
         """Load an object.
 
         Parameters
         ----------
         path:
             Path to load object from.
```

### Comparing `etna-2.0.0/etna/core/saving.py` & `etna-2.1.0/etna/core/saving.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pathlib
 from abc import ABC
 from abc import abstractmethod
-from typing import Any
+
+from typing_extensions import Self
 
 
 class AbstractSaveable(ABC):
     """Abstract class with methods for saving, loading objects."""
 
     @abstractmethod
     def save(self, path: pathlib.Path):
@@ -16,15 +17,15 @@
         path:
             Path to save object to.
         """
         pass
 
     @classmethod
     @abstractmethod
-    def load(cls, path: pathlib.Path) -> Any:
+    def load(cls, path: pathlib.Path) -> Self:
         """Load an object.
 
         Parameters
         ----------
         path:
             Path to load object from.
         """
```

### Comparing `etna-2.0.0/etna/core/utils.py` & `etna-2.1.0/etna/core/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/datasets/__init__.py` & `etna-2.1.0/etna/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/datasets/datasets_generation.py` & `etna-2.1.0/etna/datasets/datasets_generation.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/datasets/hierarchical_structure.py` & `etna-2.1.0/etna/datasets/hierarchical_structure.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/datasets/tsdataset.py` & `etna-2.1.0/etna/datasets/tsdataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,29 +226,31 @@
         first_valid_idx = df.first_valid_index()
         df = df.loc[first_valid_idx:]
         return df
 
     def make_future(
         self, future_steps: int, transforms: Sequence["Transform"] = (), tail_steps: int = 0
     ) -> "TSDataset":
-        """Return new TSDataset with future steps.
+        """Return new TSDataset with features extended into the future.
+
+        The result dataset doesn't contain quantiles and target components.
 
         Parameters
         ----------
         future_steps:
-            number of timestamp in the future to build features for.
+            number of steps to extend dataset into the future.
         transforms:
             sequence of transforms to be applied.
         tail_steps:
-            number of timestamp for context to build features for.
+            number of steps to keep from the tail of the original dataset.
 
         Returns
         -------
         :
-            dataset with features in the future.
+            dataset with features extended into the.
 
         Examples
         --------
         >>> from etna.datasets import generate_const_df
         >>> df = generate_const_df(
         ...    periods=30, start_time="2021-06-01",
         ...    n_segments=2, scale=1
@@ -291,30 +293,39 @@
                     regressors_index = self.df_exog.loc[:, pd.IndexSlice[segment, self.regressors]].index
                     if not np.all(future_dates.isin(regressors_index)):
                         warnings.warn(
                             f"Some regressors don't have enough values in segment {segment}, "
                             f"NaN-s will be used for missing values"
                         )
 
+        # remove components and quantiles
+        # it should be done if we have quantiles and components in raw_df
+        # TODO: fix this after making quantiles to work like components, with special methods
+        if len(self.target_components_names) > 0:
+            df = df.drop(columns=list(self.target_components_names), level="feature")
+        if len(self.target_quantiles_names) > 0:
+            df = df.drop(columns=list(self.target_quantiles_names), level="feature")
+
         # Here only df is required, other metadata is not necessary to build the dataset
         ts = TSDataset(df=df, freq=self.freq)
         for transform in transforms:
             tslogger.log(f"Transform {repr(transform)} is applied to dataset")
             transform.transform(ts)
         df = ts.to_pandas()
 
         future_dataset = df.tail(future_steps + tail_steps).copy(deep=True)
 
         future_dataset = future_dataset.sort_index(axis=1, level=(0, 1))
-        future_ts = TSDataset(df=future_dataset, freq=self.freq)
+        future_ts = TSDataset(df=future_dataset, freq=self.freq, hierarchical_structure=self.hierarchical_structure)
 
         # can't put known_future into constructor, _check_known_future fails with df_exog=None
         future_ts.known_future = deepcopy(self.known_future)
         future_ts._regressors = deepcopy(self.regressors)
-        future_ts.df_exog = self.df_exog
+        if self.df_exog is not None:
+            future_ts.df_exog = self.df_exog.copy(deep=True)
         return future_ts
 
     def tsdataset_idx_slice(self, start_idx: Optional[int] = None, end_idx: Optional[int] = None) -> "TSDataset":
         """Return new TSDataset with integer-location based indexing.
 
         Parameters
         ----------
@@ -329,16 +340,17 @@
             TSDataset based on indexing slice.
         """
         df_slice = self.df.iloc[start_idx:end_idx].copy(deep=True)
         tsdataset_slice = TSDataset(df=df_slice, freq=self.freq)
         # can't put known_future into constructor, _check_known_future fails with df_exog=None
         tsdataset_slice.known_future = deepcopy(self.known_future)
         tsdataset_slice._regressors = deepcopy(self.regressors)
-        tsdataset_slice.df_exog = self.df_exog
-        tsdataset_slice._target_components_names = self._target_components_names
+        if self.df_exog is not None:
+            tsdataset_slice.df_exog = self.df_exog.copy(deep=True)
+        tsdataset_slice._target_components_names = deepcopy(self._target_components_names)
         return tsdataset_slice
 
     @staticmethod
     def _check_known_future(
         known_future: Union[Literal["all"], Sequence], df_exog: Optional[pd.DataFrame]
     ) -> List[str]:
         """Check that ``known_future`` corresponds to ``df_exog`` and returns initial list of regressors."""
@@ -808,15 +820,23 @@
         return_hierarchy:
             If true, returns the hierarchical structure
 
         Returns
         -------
         :
             Dataframe in wide format and optionally hierarchical structure
+
+        Raises
+        ------
+        ValueError
+            If ``level_columns`` is empty
         """
+        if len(level_columns) == 0:
+            raise ValueError("Value of level_columns shouldn't be empty!")
+
         df_copy = df.copy(deep=True)
         df_copy["segment"] = df_copy[level_columns].astype("string").agg(sep.join, axis=1)
         if not keep_level_columns:
             df_copy.drop(columns=level_columns, inplace=True)
         df_copy = TSDataset.to_dataset(df_copy)
 
         hierarchical_structure = None
@@ -971,29 +991,29 @@
             df=train_df,
             df_exog=self.df_exog,
             freq=self.freq,
             known_future=self.known_future,
             hierarchical_structure=self.hierarchical_structure,
         )
         train.raw_df = train_raw_df
-        train._regressors = self.regressors
-        train._target_components_names = self.target_components_names
+        train._regressors = deepcopy(self.regressors)
+        train._target_components_names = deepcopy(self.target_components_names)
 
         test_df = self.df[test_start_defined:test_end_defined][self.raw_df.columns]  # type: ignore
         test_raw_df = self.raw_df[train_start_defined:test_end_defined]  # type: ignore
         test = TSDataset(
             df=test_df,
             df_exog=self.df_exog,
             freq=self.freq,
             known_future=self.known_future,
             hierarchical_structure=self.hierarchical_structure,
         )
         test.raw_df = test_raw_df
-        test._regressors = self.regressors
-        test._target_components_names = self.target_components_names
+        test._regressors = deepcopy(self.regressors)
+        test._target_components_names = deepcopy(self.target_components_names)
         return train, test
 
     def update_columns_from_pandas(self, df_update: pd.DataFrame):
         """Update the existing columns in the dataset with the new values from pandas dataframe.
 
         Before updating columns in df, columns of df_update will be cropped by the last timestamp in df.
         Columns in df_exog are not updated. If you wish to update the df_exog, create the new
```

### Comparing `etna-2.0.0/etna/datasets/utils.py` & `etna-2.1.0/etna/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/ensembles/direct_ensemble.py` & `etna-2.1.0/etna/ensembles/direct_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel
 from joblib import delayed
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
 from etna.ensembles.mixins import EnsembleMixin
 from etna.ensembles.mixins import SaveEnsembleMixin
 from etna.pipeline.base import BasePipeline
 
 
 class DirectEnsemble(EnsembleMixin, SaveEnsembleMixin, BasePipeline):
     """DirectEnsemble is a pipeline that forecasts future values merging the forecasts of base pipelines.
@@ -153,7 +154,19 @@
 
         horizons = [pipeline.horizon for pipeline in self.pipelines]
         pipeline = self.pipelines[np.argmin(horizons)]
         prediction = self._predict_pipeline(
             ts=ts, pipeline=pipeline, start_timestamp=start_timestamp, end_timestamp=end_timestamp
         )
         return prediction
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get hyperparameter grid to tune.
+
+        Not implemented for this class.
+
+        Returns
+        -------
+        :
+            Grid with hyperparameters.
+        """
+        raise NotImplementedError(f"{self.__class__.__name__} doesn't support this method!")
```

### Comparing `etna-2.0.0/etna/ensembles/mixins.py` & `etna-2.1.0/etna/ensembles/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pathlib
 import tempfile
 import zipfile
 from copy import deepcopy
-from typing import Any
 from typing import List
 from typing import Optional
 
 import pandas as pd
+from typing_extensions import Self
 
 from etna.core import SaveMixin
 from etna.core import load
 from etna.datasets import TSDataset
 from etna.loggers import tslogger
 from etna.pipeline.base import BasePipeline
 
@@ -109,15 +109,15 @@
                 for i, pipeline in enumerate(pipelines):
                     save_name = f"{i:0{num_digits}d}.zip"
                     pipeline_save_path = pipelines_dir / save_name
                     pipeline.save(pipeline_save_path)
                     archive.write(pipeline_save_path, f"pipelines/{save_name}")
 
     @classmethod
-    def load(cls, path: pathlib.Path, ts: Optional[TSDataset] = None) -> Any:
+    def load(cls, path: pathlib.Path, ts: Optional[TSDataset] = None) -> Self:
         """Load an object.
 
         Parameters
         ----------
         path:
             Path to load object from.
         ts:
```

### Comparing `etna-2.0.0/etna/ensembles/stacking_ensemble.py` & `etna-2.1.0/etna/ensembles/stacking_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from joblib import Parallel
 from joblib import delayed
 from sklearn.base import RegressorMixin
 from sklearn.linear_model import LinearRegression
 from typing_extensions import Literal
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
 from etna.ensembles.mixins import EnsembleMixin
 from etna.ensembles.mixins import SaveEnsembleMixin
 from etna.loggers import tslogger
 from etna.metrics import MAE
 from etna.pipeline.base import BasePipeline
 
 
@@ -88,15 +89,15 @@
         Raises
         ------
         ValueError:
             If the number of the pipelines is less than 2 or pipelines have different horizons.
         """
         self._validate_pipeline_number(pipelines=pipelines)
         self.pipelines = pipelines
-        self.final_model = LinearRegression() if final_model is None else final_model
+        self.final_model = LinearRegression(positive=True) if final_model is None else final_model
         self._validate_backtest_n_folds(n_folds)
         self.n_folds = n_folds
         self.features_to_use = features_to_use
         self.filtered_features_for_final_model: Union[None, Set[str]] = None
         self.n_jobs = n_jobs
         if joblib_params is None:
             self.joblib_params = dict(verbose=11, backend="multiprocessing", mmap_mode="c")
@@ -170,15 +171,15 @@
 
     def _make_features(
         self, ts: TSDataset, forecasts: List[TSDataset], train: bool = False
     ) -> Tuple[pd.DataFrame, Optional[pd.Series]]:
         """Prepare features for the ``final_model``."""
         # Stack targets from the forecasts
         targets = [
-            forecast[:, :, "target"].rename({"target": f"regressor_target_{i}"}, axis=1)
+            forecast[:, :, "target"].rename({"target": f"regressor_target_{i}"}, level="feature", axis=1)
             for i, forecast in enumerate(forecasts)
         ]
         targets = pd.concat(targets, axis=1)
 
         # Get features from filtered_features_for_final_model
         features = pd.DataFrame()
         if self.filtered_features_for_final_model is not None:
@@ -259,7 +260,19 @@
             delayed(self._predict_pipeline)(
                 ts=ts, pipeline=pipeline, start_timestamp=start_timestamp, end_timestamp=end_timestamp
             )
             for pipeline in self.pipelines
         )
         prediction = self._process_forecasts(ts=ts, forecasts=predictions)
         return prediction
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get hyperparameter grid to tune.
+
+        Not implemented for this class.
+
+        Returns
+        -------
+        :
+            Grid with hyperparameters.
+        """
+        raise NotImplementedError(f"{self.__class__.__name__} doesn't support this method!")
```

### Comparing `etna-2.0.0/etna/ensembles/voting_ensemble.py` & `etna-2.1.0/etna/ensembles/voting_ensemble.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from joblib import Parallel
 from joblib import delayed
 from sklearn.ensemble import RandomForestRegressor
 from typing_extensions import Literal
 
 from etna.analysis.feature_relevance.relevance_table import TreeBasedRegressor
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
 from etna.ensembles.mixins import EnsembleMixin
 from etna.ensembles.mixins import SaveEnsembleMixin
 from etna.loggers import tslogger
 from etna.metrics import MAE
 from etna.pipeline.base import BasePipeline
 
 
@@ -230,7 +231,19 @@
             delayed(self._predict_pipeline)(
                 ts=ts, pipeline=pipeline, start_timestamp=start_timestamp, end_timestamp=end_timestamp
             )
             for pipeline in self.pipelines
         )
         predictions = self._vote(forecasts=predictions)
         return predictions
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get hyperparameter grid to tune.
+
+        Not implemented for this class.
+
+        Returns
+        -------
+        :
+            Grid with hyperparameters.
+        """
+        raise NotImplementedError(f"{self.__class__.__name__} doesn't support this method!")
```

### Comparing `etna-2.0.0/etna/experimental/change_points/regularization_search.py` & `etna-2.1.0/etna/experimental/change_points/regularization_search.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/experimental/classification/classification.py` & `etna-2.1.0/etna/experimental/classification/classification.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/experimental/classification/feature_extraction/base.py` & `etna-2.1.0/etna/experimental/classification/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/experimental/classification/feature_extraction/tsfresh.py` & `etna-2.1.0/etna/experimental/classification/feature_extraction/tsfresh.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from etna import SETTINGS
 
-if SETTINGS.tsfresh_required:
+if SETTINGS.classification_required:
     from tsfresh import extract_features
     from tsfresh.feature_extraction.settings import MinimalFCParameters
 
 from etna.experimental.classification.feature_extraction.base import BaseTimeSeriesFeatureExtractor
 
 
 class TSFreshFeatureExtractor(BaseTimeSeriesFeatureExtractor):
```

### Comparing `etna-2.0.0/etna/experimental/classification/feature_extraction/weasel.py` & `etna-2.1.0/etna/experimental/classification/feature_extraction/weasel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,33 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 from numpy.lib.stride_tricks import sliding_window_view
-from pyts.approximation import SymbolicFourierApproximation
-from pyts.transformation import WEASEL
 from scipy.sparse import coo_matrix
 from scipy.sparse import csr_matrix
 from scipy.sparse import hstack
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.feature_selection import chi2
 from typing_extensions import Literal
 
+from etna import SETTINGS
 from etna.experimental.classification.feature_extraction.base import BaseTimeSeriesFeatureExtractor
 from etna.experimental.classification.utils import padd_single_series
 
+if SETTINGS.classification_required:
+    from pyts.approximation import SymbolicFourierApproximation
+    from pyts.transformation import WEASEL
+else:
+    from unittest.mock import Mock
+
+    WEASEL = Mock  # type: ignore
+
 
 class CustomWEASEL(WEASEL):
     """Improved version of WEASEL transform to work with the series of different length."""
 
     def __init__(
         self,
         padding_value: Union[float, Literal["back_fill"]],
@@ -202,14 +209,17 @@
             Array with time series.
 
         Returns
         -------
         :
             Transformed input data.
         """
+        if self._padding_expected_len is None:
+            raise ValueError("Transform is not fitted!")
+
         n_samples = len(x)
         window_sizes, window_steps = self._check_params(self._min_series_len)
         for i in range(len(x)):
             x[i] = (
                 x[i]
                 if len(x[i]) >= max(window_sizes)
                 else padd_single_series(
```

### Comparing `etna-2.0.0/etna/experimental/classification/predictability.py` & `etna-2.1.0/etna/experimental/classification/predictability.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/experimental/classification/utils.py` & `etna-2.1.0/etna/experimental/classification/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/libs/pmdarima_utils/arima.py` & `etna-2.1.0/etna/libs/pmdarima_utils/arima.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/libs/tsfresh/defaults.py` & `etna-2.1.0/etna/libs/tsfresh/defaults.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,17 +12,23 @@
 Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
-# Note: Copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/ff69073bbb4df787fcbf277a611c6b40632e767d/tsfresh/defaults.py)
+# Note: Copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/v0.20.0/tsfresh/defaults.py)
+
+import os
+from multiprocessing import cpu_count
+
+n_cores = int(os.getenv("NUMBER_OF_CPUS") or cpu_count())
+
 CHUNKSIZE = None
-N_PROCESSES = 1
+N_PROCESSES = max(1, n_cores // 2)
 PROFILING = False
 PROFILING_SORTING = "cumulative"
 PROFILING_FILENAME = "profile.txt"
 IMPUTE_FUNCTION = None
 DISABLE_PROGRESSBAR = False
 SHOW_WARNINGS = False
 PARALLELISATION = True
```

### Comparing `etna-2.0.0/etna/libs/tsfresh/distribution.py` & `etna-2.1.0/etna/libs/tsfresh/distribution.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
+# Note: Originally copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/v0.20.0/tsfresh/utilities/distribution.py)
+
 import warnings
-# Note: Originally copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/ff69073bbb4df787fcbf277a611c6b40632e767d/tsfresh/utilities/distribution.py)
+
+
 def initialize_warnings_in_workers(show_warnings):
     """
     Small helper function to initialize warnings module in multiprocessing workers.
 
     On Windows, Python spawns fresh processes which do not inherit from warnings
     state, so warnings must be enabled/disabled before running computations.
```

### Comparing `etna-2.0.0/etna/libs/tsfresh/relevance.py` & `etna-2.1.0/etna/libs/tsfresh/relevance.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,34 @@
 Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
+# Note: Originally copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/v0.20.0/tsfresh/feature_selection/relevance.py)
 
-from multiprocessing import Pool
 import warnings
+from functools import partial, reduce
+from multiprocessing import Pool
 
 import numpy as np
 import pandas as pd
-from functools import partial, reduce
 from statsmodels.stats.multitest import multipletests
 
 from etna.libs.tsfresh import defaults
 from etna.libs.tsfresh.significance_tests import (
+    target_binary_feature_binary_test,
     target_binary_feature_real_test,
     target_real_feature_binary_test,
     target_real_feature_real_test,
-    target_binary_feature_binary_test,
 )
 from etna.libs.tsfresh.distribution import initialize_warnings_in_workers
 
-# Note: Originally copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/ff69073bbb4df787fcbf277a611c6b40632e767d/tsfresh/feature_selection/relevance.py)
+
 def calculate_relevance_table(
     X,
     y,
     ml_task="auto",
     multiclass=False,
     n_significant=1,
     n_jobs=defaults.N_PROCESSES,
@@ -195,15 +196,15 @@
 
     with warnings.catch_warnings():
         if not show_warnings:
             warnings.simplefilter("ignore")
         else:
             warnings.simplefilter("default")
 
-        if n_jobs == 0:
+        if n_jobs == 0 or n_jobs == 1:
             map_function = map
         else:
             pool = Pool(
                 processes=n_jobs,
                 initializer=initialize_warnings_in_workers,
                 initargs=(show_warnings,),
             )
@@ -230,15 +231,15 @@
                 "[test_feature_significance] Constant features: {}".format(
                     ", ".join(map(str, table_const.feature))
                 ),
                 RuntimeWarning,
             )
 
         if len(table_const) == len(relevance_table):
-            if n_jobs != 0:
+            if n_jobs < 0 or n_jobs > 1:
                 pool.close()
                 pool.terminate()
                 pool.join()
             return table_const
 
         if ml_task == "classification":
             tables = []
@@ -297,15 +298,15 @@
                 _test_real_feature,
                 _test_binary_feature,
                 hypotheses_independent,
                 fdr_level,
                 map_function,
             )
 
-        if n_jobs != 0:
+        if n_jobs < 0 or n_jobs > 1:
             pool.close()
             pool.terminate()
             pool.join()
 
         # set constant features to be irrelevant for all classes in multiclass case
         if multiclass:
             for column in relevance_table.filter(regex="^relevant_", axis=1).columns:
```

### Comparing `etna-2.0.0/etna/libs/tsfresh/relevance.pyi` & `etna-2.1.0/etna/libs/tsfresh/relevance.pyi`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/libs/tsfresh/significance_tests.py` & `etna-2.1.0/etna/libs/tsfresh/significance_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
+# Note: Originally copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/v0.20.0/tsfresh/feature_selection/significance_tests.py)
+
+import warnings
 from builtins import str
+
 import numpy as np
 import pandas as pd
 from scipy import stats
-import warnings
 
-# Note: Originally copied from tsfresh package (https://github.com/blue-yonder/tsfresh/blob/ff69073bbb4df787fcbf277a611c6b40632e767d/tsfresh/feature_selection/significance_tests.py)
+
 def target_binary_feature_binary_test(x, y):
     """
     Calculate the feature significance of a binary feature to a binary target as a p-value.
     Use the two-sided univariate fisher test from :func:`~scipy.stats.fisher_exact` for this.
 
     :param x: the binary feature vector
     :type x: pandas.Series
@@ -52,16 +55,15 @@
 
     # Calculate contingency table
     n_y1_x0 = np.sum(y[x == x0] == y1)
     n_y0_x0 = len(y[x == x0]) - n_y1_x0
     n_y1_x1 = np.sum(y[x == x1] == y1)
     n_y0_x1 = len(y[x == x1]) - n_y1_x1
 
-    table = np.array([[n_y1_x1, n_y1_x0],
-                      [n_y0_x1, n_y0_x0]])
+    table = np.array([[n_y1_x1, n_y1_x0], [n_y0_x1, n_y0_x0]])
 
     # Perform the Fisher test
     oddsratio, p_value = stats.fisher_exact(table, alternative="two-sided")
 
     return p_value
 
 
@@ -95,25 +97,29 @@
     # Extract the unique values
     y0, y1 = np.unique(y.values)
 
     # Divide feature according to target
     x_y1 = x[y == y1]
     x_y0 = x[y == y0]
 
-    if test == 'mann':
+    if test == "mann":
         # Perform Mann-Whitney-U test
-        U, p_mannwhitu = stats.mannwhitneyu(x_y1, x_y0, use_continuity=True, alternative='two-sided')
+        U, p_mannwhitu = stats.mannwhitneyu(
+            x_y1, x_y0, use_continuity=True, alternative="two-sided"
+        )
         return p_mannwhitu
-    elif test == 'smir':
+    elif test == "smir":
         # Perform Kolmogorov-Smirnov test
         KS, p_ks = stats.ks_2samp(x_y1, x_y0)
         return p_ks
     else:
-        raise ValueError("Please use a valid entry for test_for_binary_target_real_feature. " +
-                         "Valid entries are 'mann' and 'smir'.")
+        raise ValueError(
+            "Please use a valid entry for test_for_binary_target_real_feature. "
+            + "Valid entries are 'mann' and 'smir'."
+        )
 
 
 def target_real_feature_binary_test(x, y):
     """
     Calculate the feature significance of a binary feature to a real-valued target as a p-value.
     Use the `Kolmogorov-Smirnov` test from from :func:`~scipy.stats.ks_2samp` for this.
 
@@ -204,17 +210,20 @@
 
     :raises: ``ValueError`` if the values are not binary.
     """
     if not set(y) == {0, 1}:
         if len(set(y)) > 2:
             raise ValueError("Target is not binary!")
 
-        warnings.warn("The binary target should have "
-                      "values 1 and 0 (or True and False). "
-                      "Instead found" + str(set(y)), RuntimeWarning)
+        warnings.warn(
+            "The binary target should have "
+            "values 1 and 0 (or True and False). "
+            "Instead found" + str(set(y)),
+            RuntimeWarning,
+        )
 
 
 def __check_for_binary_feature(x):
     """
     Helper function to check if a feature column is binary.
     Checks if only the values true and false (or 0 and 1) are present in the values.
 
@@ -224,27 +233,32 @@
     :return: None
     :rtype: None
 
     :raises: ``ValueError`` if the values are not binary.
     """
     if not set(x) == {0, 1}:
         if len(set(x)) > 2:
-            raise ValueError("[target_binary_feature_binary_test] Feature is not binary!")
-
-        warnings.warn("A binary feature should have only "
-                      "values 1 and 0 (incl. True and False). "
-                      "Instead found " + str(set(x)) + " in feature ''" + str(x.name) + "''.", RuntimeWarning)
+            raise ValueError(
+                "[target_binary_feature_binary_test] Feature is not binary!"
+            )
+
+        warnings.warn(
+            "A binary feature should have only "
+            "values 1 and 0 (incl. True and False). "
+            "Instead found " + str(set(x)) + " in feature ''" + str(x.name) + "''.",
+            RuntimeWarning,
+        )
 
 
 def _check_for_nans(x, y):
     """
     Helper function to check if target or feature contains NaNs.
     :param x: A feature
     :type x: pandas.Series
     :param y: The target
     :type y: pandas.Series
     :raises: `ValueError` if target or feature contains NaNs.
     """
     if np.isnan(x.values).any():
-        raise ValueError('Feature {} contains NaN values'.format(x.name))
+        raise ValueError("Feature {} contains NaN values".format(x.name))
     elif np.isnan(y.values).any():
-        raise ValueError('Target contains NaN values')
+        raise ValueError("Target contains NaN values")
```

### Comparing `etna-2.0.0/etna/loggers/__init__.py` & `etna-2.1.0/etna/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/loggers/base.py` & `etna-2.1.0/etna/loggers/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/loggers/console_logger.py` & `etna-2.1.0/etna/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/loggers/file_logger.py` & `etna-2.1.0/etna/loggers/file_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from botocore.exceptions import ClientError
 
 from etna.loggers.base import BaseLogger
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
-DATETIME_FORMAT = "%Y-%m-%dT%H-%M-%S"
+DATETIME_FORMAT = "%Y-%m-%dT%H-%M-%S-%f"
 
 
 class BaseFileLogger(BaseLogger):
     """Base logger for logging files."""
 
     def log(self, msg: Union[str, Dict[str, Any]], **kwargs):
         """
```

### Comparing `etna-2.0.0/etna/loggers/wandb_logger.py` & `etna-2.1.0/etna/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/metrics/__init__.py` & `etna-2.1.0/etna/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/metrics/base.py` & `etna-2.1.0/etna/metrics/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/metrics/functional_metrics.py` & `etna-2.1.0/etna/metrics/functional_metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/metrics/intervals_metrics.py` & `etna-2.1.0/etna/metrics/intervals_metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/metrics/metrics.py` & `etna-2.1.0/etna/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/metrics/utils.py` & `etna-2.1.0/etna/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/__init__.py` & `etna-2.1.0/etna/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/autoarima.py` & `etna-2.1.0/etna/models/autoarima.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/base.py` & `etna-2.1.0/etna/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from etna import SETTINGS
-from etna.core import AbstractSaveable
 from etna.core import SaveMixin
 from etna.core.mixins import BaseMixin
 from etna.datasets.tsdataset import TSDataset
+from etna.distributions import BaseDistribution
 from etna.loggers import tslogger
 from etna.models.decorators import log_decorator
 from etna.models.mixins import SaveNNMixin
 
 if SETTINGS.torch_required:
     import torch
     from pytorch_lightning import LightningModule
@@ -32,15 +32,15 @@
 else:
     from unittest.mock import Mock
 
     LightningModule = Mock  # type: ignore
     SaveNNMixin = Mock  # type: ignore
 
 
-class AbstractModel(SaveMixin, AbstractSaveable, ABC, BaseMixin):
+class AbstractModel(SaveMixin, ABC, BaseMixin):
     """Interface for model with fit method."""
 
     @property
     @abstractmethod
     def context_size(self) -> int:
         """Context size of the model. Determines how many history points do we ask to pass to the model."""
         pass
@@ -76,14 +76,26 @@
             * if model is multi-segment, then the result is internal model
 
             * if model is per-segment, then the result is dictionary where key is segment and value is internal model
 
         """
         pass
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get grid for tuning hyperparameters.
+
+        This is default implementation with empty grid.
+
+        Returns
+        -------
+        :
+            Empty grid.
+        """
+        return {}
+
 
 class NonPredictionIntervalContextIgnorantAbstractModel(AbstractModel):
     """Interface for models that don't support prediction intervals and don't need context for prediction."""
 
     @property
     def context_size(self) -> int:
         """Context size of the model. Determines how many history points do we ask to pass to the model.
```

### Comparing `etna-2.0.0/etna/models/catboost.py` & `etna-2.1.0/etna/models/catboost.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from catboost import CatBoostRegressor
 from catboost import Pool
 
+from etna.distributions import BaseDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
 from etna.models.base import BaseAdapter
 from etna.models.base import NonPredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import MultiSegmentModelMixin
 from etna.models.mixins import NonPredictionIntervalContextIgnorantModelMixin
 from etna.models.mixins import PerSegmentModelMixin
 
 
@@ -148,14 +152,32 @@
         # encapsulate expected contribution into components
         components = shap_values[:, :-1] + shap_values[:, -1, np.newaxis] / (shap_values.shape[1] - 1)
 
         component_names = [f"target_component_{name}" for name in features.columns]
 
         return pd.DataFrame(data=components, columns=component_names)
 
+    def _params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``learning_rate``, ``depth``, ``random_strength``, ``l2_leaf_reg``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "learning_rate": FloatDistribution(low=1e-4, high=0.5, log=True),
+            "depth": IntDistribution(low=1, high=11),
+            "random_strength": FloatDistribution(low=1e-5, high=10, log=True),
+            "l2_leaf_reg": FloatDistribution(low=0.1, high=200, log=True),
+        }
+
 
 class CatBoostPerSegmentModel(
     PerSegmentModelMixin,
     NonPredictionIntervalContextIgnorantModelMixin,
     NonPredictionIntervalContextIgnorantAbstractModel,
 ):
     """Class for holding per segment Catboost model.
@@ -275,14 +297,27 @@
                 logging_level=logging_level,
                 thread_count=thread_count,
                 l2_leaf_reg=l2_leaf_reg,
                 **kwargs,
             )
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``learning_rate``, ``depth``, ``random_strength``, ``l2_leaf_reg``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return self._base_model._params_to_tune()
+
 
 class CatBoostMultiSegmentModel(
     MultiSegmentModelMixin,
     NonPredictionIntervalContextIgnorantModelMixin,
     NonPredictionIntervalContextIgnorantAbstractModel,
 ):
     """Class for holding Catboost model for all segments.
@@ -401,7 +436,20 @@
                 learning_rate=learning_rate,
                 logging_level=logging_level,
                 thread_count=thread_count,
                 l2_leaf_reg=l2_leaf_reg,
                 **kwargs,
             )
         )
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``learning_rate``, ``depth``, ``random_strength``, ``l2_leaf_reg``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return self._base_model._params_to_tune()
```

### Comparing `etna-2.0.0/etna/models/deadline_ma.py` & `etna-2.1.0/etna/models/deadline_ma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import warnings
 from enum import Enum
+from typing import Dict
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
+from typing_extensions import assert_never
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import IntDistribution
 from etna.models.base import NonPredictionIntervalContextRequiredAbstractModel
 
 
-class SeasonalityMode(Enum):
+class SeasonalityMode(str, Enum):
     """Enum for seasonality mode for DeadlineMovingAverageModel."""
 
     month = "month"
     year = "year"
 
     @classmethod
     def _missing_(cls, value):
@@ -41,15 +45,15 @@
         Length of the context is equal to the number of ``window`` months or years, depending on the ``seasonality``.
 
         Parameters
         ----------
         window:
             Number of values taken for forecast for each point.
         seasonality:
-            Only allowed monthly or annual seasonality.
+            Only allowed values are "month" and "year".
         """
         self.window = window
         self.seasonality = SeasonalityMode(seasonality)
         self._freqs_available = {"H", "D"}
         self._freq: Optional[str] = None
 
     def _validate_fitted(self):
@@ -63,14 +67,16 @@
         self._validate_fitted()
 
         cur_value = None
         if self.seasonality is SeasonalityMode.year:
             cur_value = 366
         elif self.seasonality is SeasonalityMode.month:
             cur_value = 31
+        else:
+            assert_never(self.seasonality)
 
         if self._freq == "H":
             cur_value *= 24
 
         cur_value *= self.window
 
         return cur_value
@@ -149,31 +155,34 @@
         if len(history_timestamps) == 0:
             raise ValueError(
                 "Given context isn't big enough, try to decrease context_size, prediction_size or increase length of given dataframe!"
             )
 
         if seasonality is SeasonalityMode.month:
             first_index = future_timestamps[0] - pd.DateOffset(months=window)
-
         elif seasonality is SeasonalityMode.year:
             first_index = future_timestamps[0] - pd.DateOffset(years=window)
+        else:
+            assert_never(seasonality)
 
         if first_index < history_timestamps[0]:
             raise ValueError(
                 "Given context isn't big enough, try to decrease context_size, prediction_size or increase length of given dataframe!"
             )
 
         return first_index
 
     def _get_previous_date(self, date, offset):
         """Get previous date using seasonality offset."""
         if self.seasonality == SeasonalityMode.month:
             prev_date = date - pd.DateOffset(months=offset)
         elif self.seasonality == SeasonalityMode.year:
             prev_date = date - pd.DateOffset(years=offset)
+        else:
+            assert_never(self.seasonality)
 
         return prev_date
 
     def _make_prediction_components(
         self, result_template: pd.DataFrame, context: pd.DataFrame, prediction_size: int
     ) -> pd.DataFrame:
         """Estimate prediction components using ``result_template`` as a base and ``context`` as a context."""
@@ -375,9 +384,21 @@
         ts.df = new_df
 
         if return_components:
             ts.add_target_components(target_components_df=target_components_df)
 
         return ts
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``window`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {"window": IntDistribution(low=1, high=10)}
+
 
 __all__ = ["DeadlineMovingAverageModel"]
```

### Comparing `etna-2.0.0/etna/models/decorators.py` & `etna-2.1.0/etna/models/decorators.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/holt_winters.py` & `etna-2.1.0/etna/models/holt_winters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 import numpy as np
 import pandas as pd
 from scipy.special import inv_boxcox
 from statsmodels.tsa.holtwinters import ExponentialSmoothing
 from statsmodels.tsa.holtwinters.results import HoltWintersResultsWrapper
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.models.base import BaseAdapter
 from etna.models.base import NonPredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import NonPredictionIntervalContextIgnorantModelMixin
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.utils import determine_freq
 from etna.models.utils import determine_num_steps
 from etna.models.utils import select_observations
@@ -449,17 +451,19 @@
     PerSegmentModelMixin,
     NonPredictionIntervalContextIgnorantModelMixin,
     NonPredictionIntervalContextIgnorantAbstractModel,
 ):
     """
     Holt-Winters' etna model.
 
+    This model corresponds to :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing`.
+
     Notes
     -----
-    We use :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` model from statsmodels package.
+    The model :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` is used in the implementation.
 
     This model supports in-sample and out-of-sample prediction decomposition.
     Prediction components for Holt-Winters model are: level, trend and seasonality.
     For in-sample decomposition, components are obtained directly from the fitted model. For out-of-sample,
     components estimated using an analytical form of the prediction function.
     """
 
@@ -642,26 +646,54 @@
                 smoothing_trend=self.smoothing_trend,
                 smoothing_seasonal=self.smoothing_seasonal,
                 damping_trend=self.damping_trend,
                 **self.fit_kwargs,
             )
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
 
-class HoltModel(HoltWintersModel):
+        This grid tunes parameters: ``trend``, ``damped_trend``, ``use_boxcox``.
+        If ``self.seasonal`` is not None, then it also tunes ``seasonal`` parameter.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid: Dict[str, "BaseDistribution"] = {
+            "trend": CategoricalDistribution(["add", "mul", None]),
+            "damped_trend": CategoricalDistribution([False, True]),
+            "use_boxcox": CategoricalDistribution([False, True]),
+        }
+
+        if self.seasonal is not None:
+            grid.update({"seasonal": CategoricalDistribution(["add", "mul", None])})
+
+        return grid
+
+
+class HoltModel(
+    PerSegmentModelMixin,
+    NonPredictionIntervalContextIgnorantModelMixin,
+    NonPredictionIntervalContextIgnorantAbstractModel,
+):
     """
     Holt etna model.
 
-    Restricted version of HoltWinters model.
+    This is a restricted version of :py:class:`~etna.models.holt_winters.HoltWintersModel`.
+    And it corresponds to :py:class:`statsmodels.tsa.holtwinters.Holt`.
 
     Notes
     -----
-    We use :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` model from statsmodels package.
-    They implement :py:class:`statsmodels.tsa.holtwinters.Holt` model
-    as a restricted version of :py:class:`~statsmodels.tsa.holtwinters.ExponentialSmoothing` model.
+    The model :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` is used in the implementation.
+    In statsmodels package the model :py:class:`statsmodels.tsa.holtwinters.Holt` is implemented
+    as a restricted version of :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` model.
 
     This model supports in-sample and out-of-sample prediction decomposition.
     Prediction components for Holt model are: level and trend.
     For in-sample decomposition, components are obtained directly from the fitted model. For out-of-sample,
     components estimated using an analytical form of the prediction function.
     """
 
@@ -731,39 +763,68 @@
             set then this value will be used as the value.
         damping_trend:
             The phi value of the damped method, if the value is
             set then this value will be used as the value.
         fit_kwargs:
             Additional parameters for calling :py:meth:`statsmodels.tsa.holtwinters.ExponentialSmoothing.fit`.
         """
+        self.exponential = exponential
         trend = "mul" if exponential else "add"
+        self.damped_trend = damped_trend
+        self.initialization_method = initialization_method
+        self.initial_level = initial_level
+        self.initial_trend = initial_trend
+        self.smoothing_level = smoothing_level
+        self.smoothing_trend = smoothing_trend
+        self.damping_trend = damping_trend
+        self.fit_kwargs = fit_kwargs
         super().__init__(
-            trend=trend,
-            damped_trend=damped_trend,
-            initialization_method=initialization_method,
-            initial_level=initial_level,
-            initial_trend=initial_trend,
-            smoothing_level=smoothing_level,
-            smoothing_trend=smoothing_trend,
-            damping_trend=damping_trend,
-            **fit_kwargs,
+            base_model=_HoltWintersAdapter(
+                trend=trend,
+                damped_trend=self.damped_trend,
+                initialization_method=self.initialization_method,
+                initial_level=self.initial_level,
+                initial_trend=self.initial_trend,
+                smoothing_level=self.smoothing_level,
+                smoothing_trend=self.smoothing_trend,
+                damping_trend=self.damping_trend,
+                **self.fit_kwargs,
+            )
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "exponential": CategoricalDistribution([False, True]),
+            "damped_trend": CategoricalDistribution([False, True]),
+        }
+
 
-class SimpleExpSmoothingModel(HoltWintersModel):
+class SimpleExpSmoothingModel(
+    PerSegmentModelMixin,
+    NonPredictionIntervalContextIgnorantModelMixin,
+    NonPredictionIntervalContextIgnorantAbstractModel,
+):
     """
     Exponential smoothing etna model.
 
-    Restricted version of HoltWinters model.
+    This is a restricted version of :py:class:`~etna.models.holt_winters.HoltWintersModel`.
+    And it corresponds to :py:class:`statsmodels.tsa.holtwinters.SimpleExpSmoothing`.
 
     Notes
     -----
-    We use :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` model from statsmodels package.
-    They implement :py:class:`statsmodels.tsa.holtwinters.SimpleExpSmoothing` model
-    as a restricted version of :py:class:`~statsmodels.tsa.holtwinters.ExponentialSmoothing` model.
+    The model :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` is used in the implementation.
+    In statsmodels package the model :py:class:`statsmodels.tsa.holtwinters.SimpleExpSmoothing` is implemented
+    as a restricted version of :py:class:`statsmodels.tsa.holtwinters.ExponentialSmoothing` model.
 
     This model supports in-sample and out-of-sample prediction decomposition.
     For in-sample decomposition, level component is obtained directly from the fitted model. For out-of-sample,
     it estimated using an analytical form of the prediction function.
     """
 
     def __init__(
@@ -806,13 +867,19 @@
             parameters.
         smoothing_level:
             The alpha value of the simple exponential smoothing, if the value
             is set then this value will be used as the value.
         fit_kwargs:
             Additional parameters for calling :py:meth:`statsmodels.tsa.holtwinters.ExponentialSmoothing.fit`.
         """
+        self.initialization_method = initialization_method
+        self.initial_level = initial_level
+        self.smoothing_level = smoothing_level
+        self.fit_kwargs = fit_kwargs
         super().__init__(
-            initialization_method=initialization_method,
-            initial_level=initial_level,
-            smoothing_level=smoothing_level,
-            **fit_kwargs,
+            base_model=_HoltWintersAdapter(
+                initialization_method=self.initialization_method,
+                initial_level=self.initial_level,
+                smoothing_level=self.smoothing_level,
+                **self.fit_kwargs,
+            )
         )
```

### Comparing `etna-2.0.0/etna/models/linear.py` & `etna-2.1.0/etna/models/linear.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,32 @@
+from typing import Dict
+
 import pandas as pd
 from sklearn.linear_model import ElasticNet
 from sklearn.linear_model import LinearRegression
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
+from etna.distributions import FloatDistribution
 from etna.models.base import NonPredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import MultiSegmentModelMixin
 from etna.models.mixins import NonPredictionIntervalContextIgnorantModelMixin
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.sklearn import _SklearnAdapter
 
+_LINEAR_GRID: Dict[str, BaseDistribution] = {
+    "fit_intercept": CategoricalDistribution([False, True]),
+}
+
+_ELASTIC_GRID: Dict[str, BaseDistribution] = {
+    "fit_intercept": CategoricalDistribution([False, True]),
+    "l1_ratio": FloatDistribution(low=0, high=1),
+    "alpha": FloatDistribution(low=1e-5, high=1e3, log=True),
+}
+
 
 class _LinearAdapter(_SklearnAdapter):
     def predict_components(self, df: pd.DataFrame) -> pd.DataFrame:
         """Estimate prediction components.
 
         Parameters
         ----------
@@ -60,14 +75,24 @@
         """
         self.fit_intercept = fit_intercept
         self.kwargs = kwargs
         super().__init__(
             base_model=_LinearAdapter(regressor=LinearRegression(fit_intercept=self.fit_intercept, **self.kwargs))
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return _LINEAR_GRID
+
 
 class ElasticPerSegmentModel(
     PerSegmentModelMixin,
     NonPredictionIntervalContextIgnorantModelMixin,
     NonPredictionIntervalContextIgnorantAbstractModel,
 ):
     """
@@ -113,14 +138,24 @@
                     l1_ratio=self.l1_ratio,
                     fit_intercept=self.fit_intercept,
                     **self.kwargs,
                 )
             )
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return _ELASTIC_GRID
+
 
 class LinearMultiSegmentModel(
     MultiSegmentModelMixin,
     NonPredictionIntervalContextIgnorantModelMixin,
     NonPredictionIntervalContextIgnorantAbstractModel,
 ):
     """
@@ -143,14 +178,24 @@
         """
         self.fit_intercept = fit_intercept
         self.kwargs = kwargs
         super().__init__(
             base_model=_LinearAdapter(regressor=LinearRegression(fit_intercept=self.fit_intercept, **self.kwargs))
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return _LINEAR_GRID
+
 
 class ElasticMultiSegmentModel(
     MultiSegmentModelMixin,
     NonPredictionIntervalContextIgnorantModelMixin,
     NonPredictionIntervalContextIgnorantAbstractModel,
 ):
     """
@@ -195,7 +240,17 @@
                     alpha=self.alpha,
                     l1_ratio=self.l1_ratio,
                     fit_intercept=self.fit_intercept,
                     **self.kwargs,
                 )
             )
         )
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return _ELASTIC_GRID
```

### Comparing `etna-2.0.0/etna/models/mixins.py` & `etna-2.1.0/etna/models/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Dict
 from typing import Optional
 from typing import Sequence
 
 import dill
 import numpy as np
 import pandas as pd
+from typing_extensions import Self
 
 from etna.core.mixins import SaveMixin
 from etna.datasets.tsdataset import TSDataset
 from etna.models.decorators import log_decorator
 
 
 class ModelForecastingMixin(ABC):
@@ -641,12 +642,12 @@
     def _save_state(self, archive: zipfile.ZipFile):
         import torch
 
         with archive.open("object.pt", "w") as output_file:
             torch.save(self, output_file, pickle_module=dill)
 
     @classmethod
-    def _load_state(cls, archive: zipfile.ZipFile) -> Any:
+    def _load_state(cls, archive: zipfile.ZipFile) -> Self:
         import torch
 
         with archive.open("object.pt", "r") as input_file:
             return torch.load(input_file, pickle_module=dill)
```

### Comparing `etna-2.0.0/etna/models/moving_average.py` & `etna-2.1.0/etna/models/moving_average.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/naive.py` & `etna-2.1.0/etna/models/naive.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Dict
+
+from etna.distributions import BaseDistribution
 from etna.models.seasonal_ma import SeasonalMovingAverageModel
 
 
 class NaiveModel(SeasonalMovingAverageModel):
     """Naive model predicts t-th value of series with its (t - lag) value.
 
     .. math::
@@ -23,9 +26,21 @@
         ----------
         lag: int
             lag for new value prediction
         """
         self.lag = lag
         super().__init__(window=1, seasonality=lag)
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid is empty.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {}
+
 
 __all__ = ["NaiveModel"]
```

### Comparing `etna-2.0.0/etna/models/nn/deepar.py` & `etna-2.1.0/etna/models/nn/deepar.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from typing import Sequence
 from typing import Union
 
 import pandas as pd
 
 from etna import SETTINGS
 from etna.datasets.tsdataset import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
 from etna.models.base import PredictionIntervalContextRequiredAbstractModel
 from etna.models.base import log_decorator
 from etna.models.mixins import SaveNNMixin
 from etna.models.nn.utils import PytorchForecastingDatasetBuilder
 from etna.models.nn.utils import PytorchForecastingMixin
 from etna.models.nn.utils import _DeepCopyMixin
 
@@ -236,16 +239,33 @@
             TSDataset with predictions.
         """
         raise NotImplementedError("Method predict isn't currently implemented!")
 
     def get_model(self) -> Any:
         """Get internal model that is used inside etna class.
 
-        Internal model is a model that is used inside etna to forecast segments,
-        e.g. :py:class:`catboost.CatBoostRegressor` or :py:class:`sklearn.linear_model.Ridge`.
+        Model is the instance of :py:class:`pytorch_forecasting.models.deepar.DeepAR`.
 
         Returns
         -------
         :
            Internal model
         """
         return self.model
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``hidden_size``, ``rnn_layers``, ``dropout``, ``lr``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "hidden_size": IntDistribution(low=4, high=64, step=4),
+            "rnn_layers": IntDistribution(low=1, high=3),
+            "dropout": FloatDistribution(low=0, high=0.5),
+            "lr": FloatDistribution(low=1e-5, high=1e-2, log=True),
+        }
```

### Comparing `etna-2.0.0/etna/models/nn/mlp.py` & `etna-2.1.0/etna/models/nn/mlp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 
+import numpy as np
 import pandas as pd
 from typing_extensions import TypedDict
 
 from etna import SETTINGS
+from etna.distributions import BaseDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
+from etna.models.base import DeepBaseModel
+from etna.models.base import DeepBaseNet
 
 if SETTINGS.torch_required:
     import torch
     import torch.nn as nn
 
-import numpy as np
-
-from etna.models.base import DeepBaseModel
-from etna.models.base import DeepBaseNet
-
 
 class MLPBatch(TypedDict):
     """Batch specification for MLP."""
 
     decoder_real: "torch.Tensor"
     decoder_target: "torch.Tensor"
     segment: "torch.Tensor"
@@ -105,48 +106,58 @@
 
         output = self.mlp(decoder_real)
         loss = self.loss(output, decoder_target)
         return loss, decoder_target, output
 
     def make_samples(self, df: pd.DataFrame, encoder_length: int, decoder_length: int) -> Iterable[dict]:
         """Make samples from segment DataFrame."""
+        values_real = (
+            df.select_dtypes(include=[np.number]).pipe(lambda x: x[[i for i in x.columns if i != "target"]]).values
+        )
+        values_target = df["target"].values
+        segment = df["segment"].values[0]
+
+        def _make(
+            values_target: np.ndarray, values_real: np.ndarray, segment: str, start_idx: int, decoder_length: int
+        ) -> Optional[dict]:
 
-        def _make(df: pd.DataFrame, start_idx: int, decoder_length: int) -> Optional[dict]:
             sample: Dict[str, Any] = {"decoder_real": list(), "decoder_target": list(), "segment": None}
             total_length = len(df["target"])
             total_sample_length = decoder_length
 
             if total_sample_length + start_idx > total_length:
                 return None
 
-            sample["decoder_real"] = (
-                df.select_dtypes(include=[np.number])
-                .pipe(lambda x: x[[i for i in x.columns if i != "target"]])
-                .values[start_idx : start_idx + decoder_length]
-            )
-
-            target = df["target"].values[start_idx : start_idx + decoder_length].reshape(-1, 1)
-            sample["decoder_target"] = target
-            sample["segment"] = df["segment"].values[0]
+            sample["decoder_real"] = values_real[start_idx : start_idx + decoder_length]
+            sample["decoder_target"] = values_target[start_idx : start_idx + decoder_length].reshape(-1, 1)
+            sample["segment"] = segment
             return sample
 
         start_idx = 0
         while True:
             batch = _make(
-                df=df,
+                values_target=values_target,
+                values_real=values_real,
+                segment=segment,
                 start_idx=start_idx,
                 decoder_length=decoder_length,
             )
             if batch is None:
                 break
             yield batch
             start_idx += decoder_length
         if start_idx < len(df):
             resid_length = len(df) - decoder_length
-            batch = _make(df=df, start_idx=resid_length, decoder_length=decoder_length)
+            batch = _make(
+                values_target=values_target,
+                values_real=values_real,
+                segment=segment,
+                start_idx=resid_length,
+                decoder_length=decoder_length,
+            )
             if batch is not None:
                 yield batch
 
     def configure_optimizers(self):
         """Optimizer configuration."""
         optimizer = torch.optim.Adam(self.parameters(), lr=self.lr, **self.optimizer_params)
         return optimizer
@@ -227,7 +238,28 @@
             test_batch_size=test_batch_size,
             train_dataloader_params=train_dataloader_params,
             test_dataloader_params=test_dataloader_params,
             val_dataloader_params=val_dataloader_params,
             trainer_params=trainer_params,
             split_params=split_params,
         )
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``lr``, ``hidden_size.i`` where i from 0 to ``len(hidden_size) - 1``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid: Dict[str, BaseDistribution] = {}
+
+        for i in range(len(self.hidden_size)):
+            key = f"hidden_size.{i}"
+            value = IntDistribution(low=4, high=64, step=4)
+            grid[key] = value
+
+        grid["lr"] = FloatDistribution(low=1e-5, high=1e-2, log=True)
+        return grid
```

### Comparing `etna-2.0.0/etna/models/nn/rnn.py` & `etna-2.1.0/etna/models/nn/rnn.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from typing_extensions import TypedDict
 
 from etna import SETTINGS
+from etna.distributions import BaseDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
+from etna.models.base import DeepBaseModel
+from etna.models.base import DeepBaseNet
 
 if SETTINGS.torch_required:
     import torch
     import torch.nn as nn
 
-from etna.models.base import DeepBaseModel
-from etna.models.base import DeepBaseNet
-
 
 class RNNBatch(TypedDict):
     """Batch specification for RNN."""
 
     encoder_real: "torch.Tensor"
     decoder_real: "torch.Tensor"
     encoder_target: "torch.Tensor"
@@ -127,60 +129,67 @@
         target_prediction = self.projection(target_prediction)  # (batch_size, decoder_length, 1)
 
         loss = self.loss(target_prediction, decoder_target)
         return loss, decoder_target, target_prediction
 
     def make_samples(self, df: pd.DataFrame, encoder_length: int, decoder_length: int) -> Iterator[dict]:
         """Make samples from segment DataFrame."""
+        values_real = (
+            df.select_dtypes(include=[np.number])
+            .assign(target_shifted=df["target"].shift(1))
+            .drop(["target"], axis=1)
+            .pipe(lambda x: x[["target_shifted"] + [i for i in x.columns if i != "target_shifted"]])
+            .values
+        )
+        values_target = df["target"].values
+        segment = df["segment"].values[0]
+
+        def _make(
+            values_real: np.ndarray,
+            values_target: np.ndarray,
+            segment: str,
+            start_idx: int,
+            encoder_length: int,
+            decoder_length: int,
+        ) -> Optional[dict]:
 
-        def _make(df: pd.DataFrame, start_idx: int, encoder_length: int, decoder_length: int) -> Optional[dict]:
             sample: Dict[str, Any] = {
                 "encoder_real": list(),
                 "decoder_real": list(),
                 "encoder_target": list(),
                 "decoder_target": list(),
                 "segment": None,
             }
-            total_length = len(df["target"])
+            total_length = len(values_target)
             total_sample_length = encoder_length + decoder_length
 
             if total_sample_length + start_idx > total_length:
                 return None
 
             # Get shifted target and concatenate it with real values features
-            sample["decoder_real"] = (
-                df.select_dtypes(include=[np.number])
-                .pipe(lambda x: x[["target"] + [i for i in x.columns if i != "target"]])
-                .values[start_idx + encoder_length : start_idx + encoder_length + decoder_length]
-            )
-            sample["decoder_real"][:, 0] = (
-                df["target"].shift(1).values[start_idx + encoder_length : start_idx + encoder_length + decoder_length]
-            )
+            sample["decoder_real"] = values_real[start_idx + encoder_length : start_idx + total_sample_length]
 
             # Get shifted target and concatenate it with real values features
-            sample["encoder_real"] = (
-                df.select_dtypes(include=[np.number])
-                .pipe(lambda x: x[["target"] + [i for i in x.columns if i != "target"]])
-                .values[start_idx : start_idx + encoder_length]
-            )
-            sample["encoder_real"][:, 0] = df["target"].shift(1).values[start_idx : start_idx + encoder_length]
+            sample["encoder_real"] = values_real[start_idx : start_idx + encoder_length]
             sample["encoder_real"] = sample["encoder_real"][1:]
 
-            target = df["target"].values[start_idx : start_idx + encoder_length + decoder_length].reshape(-1, 1)
+            target = values_target[start_idx : start_idx + encoder_length + decoder_length].reshape(-1, 1)
             sample["encoder_target"] = target[1:encoder_length]
             sample["decoder_target"] = target[encoder_length:]
 
-            sample["segment"] = df["segment"].values[0]
+            sample["segment"] = segment
 
             return sample
 
         start_idx = 0
         while True:
             batch = _make(
-                df=df,
+                values_target=values_target,
+                values_real=values_real,
+                segment=segment,
                 start_idx=start_idx,
                 encoder_length=encoder_length,
                 decoder_length=decoder_length,
             )
             if batch is None:
                 break
             yield batch
@@ -274,7 +283,25 @@
             test_batch_size=test_batch_size,
             train_dataloader_params=train_dataloader_params,
             test_dataloader_params=test_dataloader_params,
             val_dataloader_params=val_dataloader_params,
             trainer_params=trainer_params,
             split_params=split_params,
         )
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``num_layers``, ``hidden_size``, ``lr``, ``encoder_length``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "num_layers": IntDistribution(low=1, high=3),
+            "hidden_size": IntDistribution(low=4, high=64, step=4),
+            "lr": FloatDistribution(low=1e-5, high=1e-2, log=True),
+            "encoder_length": IntDistribution(low=1, high=20),
+        }
```

### Comparing `etna-2.0.0/etna/models/nn/tft.py` & `etna-2.1.0/etna/models/nn/tft.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from typing import Sequence
 from typing import Union
 
 import pandas as pd
 
 from etna import SETTINGS
 from etna.datasets.tsdataset import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
 from etna.models.base import PredictionIntervalContextRequiredAbstractModel
 from etna.models.base import log_decorator
 from etna.models.mixins import SaveNNMixin
 from etna.models.nn.utils import PytorchForecastingDatasetBuilder
 from etna.models.nn.utils import PytorchForecastingMixin
 from etna.models.nn.utils import _DeepCopyMixin
 
@@ -265,16 +268,34 @@
             TSDataset with predictions.
         """
         raise NotImplementedError("Method predict isn't currently implemented!")
 
     def get_model(self) -> Any:
         """Get internal model that is used inside etna class.
 
-        Internal model is a model that is used inside etna to forecast segments,
-        e.g. :py:class:`catboost.CatBoostRegressor` or :py:class:`sklearn.linear_model.Ridge`.
+        Model is the instance of :py:class:`pytorch_forecasting.models.temporal_fusion_transformer.TemporalFusionTransformer`.
 
         Returns
         -------
         :
            Internal model
         """
         return self.model
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``hidden_size``, ``lstm_layers``, ``dropout``, ``attention_head_size``, ``lr``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "hidden_size": IntDistribution(low=4, high=64, step=4),
+            "lstm_layers": IntDistribution(low=1, high=3),
+            "dropout": FloatDistribution(low=0, high=0.5),
+            "attention_head_size": IntDistribution(low=2, high=8, step=2),
+            "lr": FloatDistribution(low=1e-5, high=1e-2, log=True),
+        }
```

### Comparing `etna-2.0.0/etna/models/nn/utils.py` & `etna-2.1.0/etna/models/nn/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self.add_encoder_length = add_encoder_length
         self.allow_missing_timesteps = allow_missing_timesteps
         self.target_normalizer = target_normalizer
         self.categorical_encoders = categorical_encoders if categorical_encoders else {}
         self.constant_fill_strategy = constant_fill_strategy if constant_fill_strategy else []
         self.lags = lags if lags else {}
         self.scalers = scalers if scalers else {}
-        self.pf_dataset_predict: Optional[TimeSeriesDataSet] = None
+        self.pf_dataset_params: Optional[Dict[str, Any]] = None
 
     def _time_encoder(self, values: List[int]) -> Dict[int, int]:
         encoded_unix_times = dict()
         for idx, value in enumerate(sorted(values)):
             encoded_unix_times[value] = idx
         return encoded_unix_times
 
@@ -162,34 +162,53 @@
             scalers=self.scalers,
         )
 
         self.pf_dataset_params = pf_dataset.get_parameters()
 
         return pf_dataset
 
-    def create_inference_dataset(self, ts: TSDataset) -> TimeSeriesDataSet:
+    def create_inference_dataset(self, ts: TSDataset, horizon: int) -> TimeSeriesDataSet:
         """Create inference dataset.
 
+        This method should be used only after ``create_train_dataset`` that is used during model training.
+
         Parameters
         ----------
         ts:
             Time series dataset.
+        horizon:
+            Size of prediction to make.
+
+        Raises
+        ------
+        ValueError:
+            if method was used before ``create_train_dataset``
         """
+        if self.pf_dataset_params is None:
+            raise ValueError(
+                "This method should only be called after create_train_dataset. Try to train the model that uses this builder."
+            )
+
         df_flat = ts.to_pandas(flatten=True)
         df_flat = df_flat[df_flat.timestamp >= self.min_timestamp]
         df_flat["target"] = df_flat["target"].fillna(0)
 
         df_flat["time_idx"] = df_flat["timestamp"].apply(lambda x: determine_num_steps(self.min_timestamp, x, ts.freq))
 
         if self.time_varying_known_categoricals:
             for feature_name in self.time_varying_known_categoricals:
                 df_flat[feature_name] = df_flat[feature_name].astype(str)
 
+        # `TimeSeriesDataSet.from_parameters` in predict mode ignores `min_prediction_length`,
+        # and we can change prediction size only by changing `max_prediction_length`
+        dataset_params = deepcopy(self.pf_dataset_params)
+        dataset_params["max_prediction_length"] = horizon
+
         pf_inference_dataset = TimeSeriesDataSet.from_parameters(
-            self.pf_dataset_params, df_flat, predict=True, stop_randomization=True
+            dataset_params, df_flat, predict=True, stop_randomization=True
         )
         return pf_inference_dataset
 
 
 class PytorchForecastingMixin:
     """Mixin for Pytorch Forecasting models."""
 
@@ -262,15 +281,15 @@
             )
         else:
             pass
 
         if len(ts.df) != horizon + self.encoder_length:
             raise ValueError("Length of dataset must be equal to horizon + max_encoder_length")
 
-        pf_dataset_inference = self.dataset_builder.create_inference_dataset(ts)
+        pf_dataset_inference = self.dataset_builder.create_inference_dataset(ts, horizon)
 
         prediction_dataloader: DataLoader = pf_dataset_inference.to_dataloader(
             train=False, batch_size=self.test_batch_size
         )
 
         # shape (segments, encoder_length)
         predicts = self.model.predict(prediction_dataloader).numpy()
```

### Comparing `etna-2.0.0/etna/models/prophet.py` & `etna-2.1.0/etna/models/prophet.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from typing import Sequence
 from typing import Set
 from typing import Union
 
 import pandas as pd
 
 from etna import SETTINGS
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
+from etna.distributions import FloatDistribution
 from etna.models.base import BaseAdapter
 from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.mixins import PredictionIntervalContextIgnorantModelMixin
 
 if SETTINGS.prophet_required:
     from prophet import Prophet
@@ -447,7 +450,27 @@
                 mcmc_samples=self.mcmc_samples,
                 interval_width=self.interval_width,
                 uncertainty_samples=self.uncertainty_samples,
                 stan_backend=self.stan_backend,
                 additional_seasonality_params=self.additional_seasonality_params,
             )
         )
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``seasonality_mode``, ``seasonality_prior_scale``, ``changepoint_prior_scale``,
+        ``changepoint_range``, ``holidays_prior_scale``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "seasonality_mode": CategoricalDistribution(["additive", "multiplicative"]),
+            "seasonality_prior_scale": FloatDistribution(low=1e-2, high=10, log=True),
+            "changepoint_prior_scale": FloatDistribution(low=1e-3, high=0.5, log=True),
+            "changepoint_range": FloatDistribution(low=0.8, high=0.95),
+            "holidays_prior_scale": FloatDistribution(low=1e-2, high=10, log=True),
+        }
```

### Comparing `etna-2.0.0/etna/models/sarimax.py` & `etna-2.1.0/etna/models/sarimax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import warnings
 from abc import abstractmethod
 from datetime import datetime
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 from statsmodels.tools.sm_exceptions import ValueWarning
 from statsmodels.tsa.statespace.sarimax import SARIMAX
 from statsmodels.tsa.statespace.sarimax import SARIMAXResultsWrapper
 from statsmodels.tsa.statespace.simulation_smoother import SimulationSmoother
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
+from etna.distributions import IntDistribution
 from etna.libs.pmdarima_utils import seasonal_prediction_with_confidence
 from etna.models.base import BaseAdapter
 from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.mixins import PredictionIntervalContextIgnorantModelMixin
 from etna.models.utils import determine_freq
 from etna.models.utils import determine_num_steps
@@ -396,17 +400,17 @@
 
     .. `SARIMAX: <https://www.statsmodels.org/stable/generated/statsmodels.tsa.statespace.sarimax.SARIMAX.html>_`
 
     """
 
     def __init__(
         self,
-        order: Tuple[int, int, int] = (2, 1, 0),
-        seasonal_order: Tuple[int, int, int, int] = (1, 1, 0, 12),
-        trend: Optional[str] = "c",
+        order: Tuple[int, int, int] = (1, 0, 0),
+        seasonal_order: Tuple[int, int, int, int] = (0, 0, 0, 0),
+        trend: Optional[str] = None,
         measurement_error: bool = False,
         time_varying_regression: bool = False,
         mle_regression: bool = True,
         simple_differencing: bool = False,
         enforce_stationarity: bool = True,
         enforce_invertibility: bool = True,
         hamilton_representation: bool = False,
@@ -574,17 +578,17 @@
     This model supports in-sample and out-of-sample prediction decomposition.
     Prediction components for SARIMAX model are: exogenous and SARIMA components.
     Decomposition is obtained directly from fitted model parameters.
     """
 
     def __init__(
         self,
-        order: Tuple[int, int, int] = (2, 1, 0),
-        seasonal_order: Tuple[int, int, int, int] = (1, 1, 0, 12),
-        trend: Optional[str] = "c",
+        order: Tuple[int, int, int] = (1, 0, 0),
+        seasonal_order: Tuple[int, int, int, int] = (0, 0, 0, 0),
+        trend: Optional[str] = None,
         measurement_error: bool = False,
         time_varying_regression: bool = False,
         mle_regression: bool = True,
         simple_differencing: bool = False,
         enforce_stationarity: bool = True,
         enforce_invertibility: bool = True,
         hamilton_representation: bool = False,
@@ -720,7 +724,39 @@
                 dates=self.dates,
                 freq=self.freq,
                 missing=self.missing,
                 validate_specification=self.validate_specification,
                 **self.kwargs,
             )
         )
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``order.0``, ``order.1``, ``order.2``, ``trend``.
+        If ``self.num_periods`` is greater than zero, then it also tunes parameters:
+        ``seasonal_order.0``, ``seasonal_order.1``, ``seasonal_order.2``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid: Dict[str, "BaseDistribution"] = {
+            "order.0": IntDistribution(low=1, high=6),
+            "order.1": IntDistribution(low=1, high=2),
+            "order.2": IntDistribution(low=1, high=6),
+            "trend": CategoricalDistribution(["n", "c", "t", "ct"]),
+        }
+
+        num_periods = self.seasonal_order[3]
+        if num_periods > 0:
+            grid.update(
+                {
+                    "seasonal_order.0": IntDistribution(low=0, high=2),
+                    "seasonal_order.1": IntDistribution(low=0, high=1),
+                    "seasonal_order.2": IntDistribution(low=0, high=1),
+                }
+            )
+
+        return grid
```

### Comparing `etna-2.0.0/etna/models/seasonal_ma.py` & `etna-2.1.0/etna/models/seasonal_ma.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import warnings
+from typing import Dict
 
 import numpy as np
 import pandas as pd
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import IntDistribution
 from etna.models.base import NonPredictionIntervalContextRequiredAbstractModel
 
 
 class SeasonalMovingAverageModel(
     NonPredictionIntervalContextRequiredAbstractModel,
 ):
     """Seasonal moving average.
@@ -229,9 +232,21 @@
 
         if return_components:
             # We use true targets as lags
             target_components_df = self._predict_components(df=df, prediction_size=prediction_size)
             ts.add_target_components(target_components_df=target_components_df)
         return ts
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``window`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {"window": IntDistribution(low=1, high=10)}
+
 
 __all__ = ["SeasonalMovingAverageModel"]
```

### Comparing `etna-2.0.0/etna/models/sklearn.py` & `etna-2.1.0/etna/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/tbats.py` & `etna-2.1.0/etna/models/tbats.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/models/utils.py` & `etna-2.1.0/etna/models/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/pipeline/assembling_pipelines.py` & `etna-2.1.0/etna/pipeline/assembling_pipelines.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/pipeline/autoregressive_pipeline.py` & `etna-2.1.0/etna/pipeline/autoregressive_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 from typing_extensions import get_args
 
 from etna.datasets import TSDataset
 from etna.models.base import ContextIgnorantModelType
 from etna.models.base import ContextRequiredModelType
 from etna.models.base import ModelType
 from etna.pipeline.base import BasePipeline
+from etna.pipeline.mixins import ModelPipelineParamsToTuneMixin
 from etna.pipeline.mixins import ModelPipelinePredictMixin
 from etna.pipeline.mixins import SaveModelPipelineMixin
 from etna.transforms import Transform
 
 
-class AutoRegressivePipeline(ModelPipelinePredictMixin, SaveModelPipelineMixin, BasePipeline):
+class AutoRegressivePipeline(
+    ModelPipelinePredictMixin, ModelPipelineParamsToTuneMixin, SaveModelPipelineMixin, BasePipeline
+):
     """Pipeline that make regressive models autoregressive.
 
     Examples
     --------
     >>> from etna.datasets import generate_periodic_df
     >>> from etna.datasets import TSDataset
     >>> from etna.models import LinearPerSegmentModel
```

### Comparing `etna-2.0.0/etna/pipeline/base.py` & `etna-2.1.0/etna/pipeline/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import warnings
 from abc import abstractmethod
 from copy import deepcopy
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import Generator
 from typing import List
@@ -18,23 +19,23 @@
 from scipy.stats import norm
 from typing_extensions import TypedDict
 from typing_extensions import assert_never
 
 from etna.core import AbstractSaveable
 from etna.core import BaseMixin
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
 from etna.loggers import tslogger
-from etna.metrics import MAE
 from etna.metrics import Metric
 from etna.metrics import MetricAggregationMode
 
 Timestamp = Union[str, pd.Timestamp]
 
 
-class CrossValidationMode(Enum):
+class CrossValidationMode(str, Enum):
     """Enum for different cross-validation modes."""
 
     expand = "expand"
     constant = "constant"
 
     @classmethod
     def _missing_(cls, value):
@@ -269,24 +270,57 @@
 
         Returns
         -------
         metrics_df, forecast_df, fold_info_df: Tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]
             Metrics dataframe, forecast dataframe and dataframe with information about folds
         """
 
+    @abstractmethod
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get hyperparameter grid to tune.
+
+        Returns
+        -------
+        :
+            Grid with hyperparameters.
+        """
+
 
 class FoldParallelGroup(TypedDict):
     """Group for parallel fold processing."""
 
     train_fold_number: int
     train_mask: FoldMask
     forecast_fold_numbers: List[int]
     forecast_masks: List[FoldMask]
 
 
+class _DummyMetric(Metric):
+    """Dummy metric that is created only for implementation of BasePipeline._forecast_prediction_interval."""
+
+    def __init__(self, mode: str = MetricAggregationMode.per_segment, **kwargs):
+        super().__init__(mode=mode, metric_fn=self._compute_metric, **kwargs)
+
+    @staticmethod
+    def _compute_metric(y_true: np.ndarray, y_pred: np.ndarray) -> float:
+        return 0.0
+
+    @property
+    def greater_is_better(self) -> bool:
+        return False
+
+    def __call__(self, y_true: TSDataset, y_pred: TSDataset) -> Union[float, Dict[str, float]]:
+        segments = set(y_true.df.columns.get_level_values("segment"))
+        metrics_per_segment = {}
+        for segment in segments:
+            metrics_per_segment[segment] = 0.0
+        metrics = self._aggregate_metrics(metrics_per_segment)
+        return metrics
+
+
 class BasePipeline(AbstractPipeline, BaseMixin):
     """Base class for pipeline."""
 
     def __init__(self, horizon: int):
         self._validate_horizon(horizon=horizon)
         self.horizon = horizon
         self.ts: Optional[TSDataset] = None
@@ -311,31 +345,52 @@
         pass
 
     def _forecast_prediction_interval(
         self, ts: TSDataset, predictions: TSDataset, quantiles: Sequence[float], n_folds: int
     ) -> TSDataset:
         """Add prediction intervals to the forecasts."""
         with tslogger.disable():
-            _, forecasts, _ = self.backtest(ts=ts, metrics=[MAE()], n_folds=n_folds)
+            _, forecasts, _ = self.backtest(ts=ts, metrics=[_DummyMetric()], n_folds=n_folds)
 
         self._add_forecast_borders(ts=ts, backtest_forecasts=forecasts, quantiles=quantiles, predictions=predictions)
 
         return predictions
 
+    @staticmethod
+    def _validate_residuals_for_interval_estimation(backtest_forecasts: TSDataset, residuals: pd.DataFrame):
+        len_backtest, num_segments = residuals.shape
+        min_timestamp = backtest_forecasts.index.min()
+        max_timestamp = backtest_forecasts.index.max()
+        non_nan_counts = np.sum(~np.isnan(residuals.values), axis=0)
+        if np.any(non_nan_counts < len_backtest):
+            warnings.warn(
+                f"There are NaNs in target on time span from {min_timestamp} to {max_timestamp}. "
+                f"It can obstruct prediction interval estimation on history data."
+            )
+        if np.any(non_nan_counts < 2):
+            raise ValueError(
+                f"There aren't enough target values to evaluate prediction intervals on history! "
+                f"For each segment there should be at least 2 points with defined value in a "
+                f"time span from {min_timestamp} to {max_timestamp}. "
+                f"You can try to increase n_folds parameter to make time span bigger."
+            )
+
     def _add_forecast_borders(
         self, ts: TSDataset, backtest_forecasts: pd.DataFrame, quantiles: Sequence[float], predictions: TSDataset
     ) -> None:
         """Estimate prediction intervals and add to the forecasts."""
         backtest_forecasts = TSDataset(df=backtest_forecasts, freq=ts.freq)
         residuals = (
             backtest_forecasts.loc[:, pd.IndexSlice[:, "target"]]
             - ts[backtest_forecasts.index.min() : backtest_forecasts.index.max(), :, "target"]
         )
 
-        sigma = np.std(residuals.values, axis=0)
+        self._validate_residuals_for_interval_estimation(backtest_forecasts=backtest_forecasts, residuals=residuals)
+        sigma = np.nanstd(residuals.values, axis=0)
+
         borders = []
         for quantile in quantiles:
             z_q = norm.ppf(q=quantile)
             border = predictions[:, :, "target"] + sigma * z_q
             border.rename({"target": f"target_{quantile:.4g}"}, inplace=True, axis=1)
             borders.append(border)
```

### Comparing `etna-2.0.0/etna/pipeline/hierarchical_pipeline.py` & `etna-2.1.0/etna/pipeline/hierarchical_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,33 +308,32 @@
             metrics_values[metric.name] = metric(y_true=y_true, y_pred=y_pred)  # type: ignore
         return metrics_values
 
     def _forecast_prediction_interval(
         self, ts: TSDataset, predictions: TSDataset, quantiles: Sequence[float], n_folds: int
     ) -> TSDataset:
         """Add prediction intervals to the forecasts."""
-        # TODO: fix this: what if during backtest KeyboardInterrupt is raised
-        self.forecast, self.raw_forecast = self.raw_forecast, self.forecast  # type: ignore
-
         if self.ts is None:
             raise ValueError("Pipeline is not fitted! Fit the Pipeline before calling forecast method.")
 
-        # TODO: rework intervals estimation for `BottomUpReconciliator`
-
-        with tslogger.disable():
-            _, forecasts, _ = self.backtest(ts=ts, metrics=[MAE()], n_folds=n_folds)
+        self.forecast, self.raw_forecast = self.raw_forecast, self.forecast  # type: ignore
+        try:
+            # TODO: rework intervals estimation for `BottomUpReconciliator`
 
-        source_ts = self.reconciliator.aggregate(ts=ts)
-        self._add_forecast_borders(
-            ts=source_ts, backtest_forecasts=forecasts, quantiles=quantiles, predictions=predictions
-        )
+            with tslogger.disable():
+                _, forecasts, _ = self.backtest(ts=ts, metrics=[MAE()], n_folds=n_folds)
 
-        self.forecast, self.raw_forecast = self.raw_forecast, self.forecast  # type: ignore
+            source_ts = self.reconciliator.aggregate(ts=ts)
+            self._add_forecast_borders(
+                ts=source_ts, backtest_forecasts=forecasts, quantiles=quantiles, predictions=predictions
+            )
+            return predictions
 
-        return predictions
+        finally:
+            self.forecast, self.raw_forecast = self.raw_forecast, self.forecast  # type: ignore
 
     def save(self, path: pathlib.Path):
         """Save the object.
 
         Parameters
         ----------
         path:
```

### Comparing `etna-2.0.0/etna/pipeline/mixins.py` & `etna-2.1.0/etna/pipeline/mixins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import pathlib
 import tempfile
 import zipfile
 from copy import deepcopy
-from typing import Any
+from typing import Dict
 from typing import Optional
 from typing import Sequence
 
 import numpy as np
 import pandas as pd
+from typing_extensions import Self
 from typing_extensions import get_args
 
 from etna.core import SaveMixin
 from etna.core import load
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
 from etna.models import ModelType
 from etna.models import NonPredictionIntervalContextIgnorantAbstractModel
 from etna.models import NonPredictionIntervalContextRequiredAbstractModel
 from etna.models import NonPredictionIntervalModelType
 from etna.models import PredictionIntervalContextIgnorantAbstractModel
 from etna.models import PredictionIntervalContextRequiredAbstractModel
 from etna.transforms import Transform
@@ -102,14 +104,45 @@
                 return_components=return_components,
             )
         else:
             raise NotImplementedError(f"Unknown model type: {self.model.__class__.__name__}!")
         return results
 
 
+class ModelPipelineParamsToTuneMixin:
+    """Mixin for pipelines with model inside with implementation of ``params_to_tune`` method."""
+
+    model: ModelType
+    transforms: Sequence[Transform]
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get hyperparameter grid to tune.
+
+        Parameters for model has prefix "model.", e.g. "model.alpha".
+
+        Parameters for transforms has prefix "transforms.idx.", e.g. "transforms.0.mode".
+
+        Returns
+        -------
+        :
+            Grid with parameters from model and transforms.
+        """
+        all_params = {}
+        for key, value in self.model.params_to_tune().items():
+            new_key = f"model.{key}"
+            all_params[new_key] = value
+
+        for i, transform in enumerate(self.transforms):
+            for key, value in transform.params_to_tune().items():
+                new_key = f"transforms.{i}.{key}"
+                all_params[new_key] = value
+
+        return all_params
+
+
 class SaveModelPipelineMixin(SaveMixin):
     """Implementation of ``AbstractSaveable`` abstract class for pipelines with model inside.
 
     It saves object to the zip archive with 4 entities:
 
     * metadata.json: contains library version and class name.
 
@@ -165,15 +198,15 @@
                 for i, transform in enumerate(transforms):
                     save_name = f"{i:0{num_digits}d}.zip"
                     transform_save_path = transforms_dir / save_name
                     transform.save(transform_save_path)
                     archive.write(transform_save_path, f"transforms/{save_name}")
 
     @classmethod
-    def load(cls, path: pathlib.Path, ts: Optional[TSDataset] = None) -> Any:
+    def load(cls, path: pathlib.Path, ts: Optional[TSDataset] = None) -> Self:
         """Load an object.
 
         Parameters
         ----------
         path:
             Path to load object from.
         ts:
```

### Comparing `etna-2.0.0/etna/pipeline/pipeline.py` & `etna-2.1.0/etna/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 from etna.datasets import TSDataset
 from etna.models.base import ContextIgnorantModelType
 from etna.models.base import ContextRequiredModelType
 from etna.models.base import ModelType
 from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
 from etna.models.base import PredictionIntervalContextRequiredAbstractModel
 from etna.pipeline.base import BasePipeline
+from etna.pipeline.mixins import ModelPipelineParamsToTuneMixin
 from etna.pipeline.mixins import ModelPipelinePredictMixin
 from etna.pipeline.mixins import SaveModelPipelineMixin
 from etna.transforms.base import Transform
 
 
-class Pipeline(ModelPipelinePredictMixin, SaveModelPipelineMixin, BasePipeline):
+class Pipeline(ModelPipelinePredictMixin, ModelPipelineParamsToTuneMixin, SaveModelPipelineMixin, BasePipeline):
     """Pipeline of transforms with a final estimator."""
 
     def __init__(self, model: ModelType, transforms: Sequence[Transform] = (), horizon: int = 1):
         """
         Create instance of Pipeline with given parameters.
 
         Parameters
```

### Comparing `etna-2.0.0/etna/reconciliation/base.py` & `etna-2.1.0/etna/reconciliation/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
             df=ts.to_pandas(features=target_names),
             mapping_matrix=self.mapping_matrix,
             source_level_segments=current_level_segments,
             target_level_segments=target_level_segments,
         )
 
         target_components_df = df_reconciled.loc[:, pd.IndexSlice[:, ts.target_components_names]]
-        df_reconciled = df_reconciled.drop(columns=list(ts.target_components_names), level="feature")
+        if len(ts.target_components_names) > 0:  # for pandas >=1.1, <1.2
+            df_reconciled = df_reconciled.drop(columns=list(ts.target_components_names), level="feature")
 
         ts_reconciled = TSDataset(
             df=df_reconciled,
             freq=ts.freq,
             df_exog=ts.df_exog,
             known_future=ts.known_future,
             hierarchical_structure=ts.hierarchical_structure,
```

### Comparing `etna-2.0.0/etna/reconciliation/bottom_up.py` & `etna-2.1.0/etna/reconciliation/bottom_up.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/reconciliation/top_down.py` & `etna-2.1.0/etna/reconciliation/top_down.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/settings.py` & `etna-2.1.0/etna/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,21 +50,29 @@
     if _module_available("prophet"):
         return True
     else:
         warnings.warn("etna[prophet] is not available, to install it, run `pip install etna[prophet]`")
         return False
 
 
-def _is_tsfresh_available():
-    if _module_available("tsfresh"):
+def _is_classification_available():
+    true_case = _module_available("pyts") & _module_available("tsfresh")
+    if true_case:
         return True
     else:
-        warnings.warn(
-            "`tsfresh` is not available, to install it, run `pip install tsfresh==0.19.0 && pip install protobuf==3.20.1`"
-        )
+        warnings.warn("etna[classification] is not available, to install it, run `pip install etna[classification]`")
+        return False
+
+
+def _is_auto_available():
+    true_case = _module_available("optuna") & _module_available("sqlalchemy")
+    if true_case:
+        return True
+    else:
+        warnings.warn("etna[auto] is not available, to install it, run `pip install etna[auto]`")
         return False
 
 
 def _get_optional_value(is_required: Optional[bool], is_available_fn: Callable, assert_msg: str) -> bool:
     if is_required is None:
         return is_available_fn()
     elif is_required:
@@ -79,15 +87,16 @@
     """etna settings."""
 
     def __init__(  # noqa: D107
         self,
         torch_required: Optional[bool] = None,
         prophet_required: Optional[bool] = None,
         wandb_required: Optional[bool] = None,
-        tsfresh_required: Optional[bool] = None,
+        classification_required: Optional[bool] = None,
+        auto_required: Optional[bool] = None,
     ):
         # True – use the package
         # None – use the package if available
         # False - block the package
         self.torch_required: bool = _get_optional_value(
             torch_required,
             _is_torch_available,
@@ -97,18 +106,23 @@
             wandb_required, _is_wandb_available, "wandb is not available, to install it, " "run `pip install wandb`."
         )
         self.prophet_required: bool = _get_optional_value(
             prophet_required,
             _is_prophet_available,
             "etna[prophet] is not available, to install it, run `pip install etna[prophet]`.",
         )
-        self.tsfresh_required: bool = _get_optional_value(
-            tsfresh_required,
-            _is_tsfresh_available,
-            "`tsfresh` is not available, to install it, run `pip install tsfresh==0.19.0 && pip install protobuf==3.20.1`",
+        self.classification_required: bool = _get_optional_value(
+            classification_required,
+            _is_classification_available,
+            "etna[classification] is not available, to install it, run `pip install etna[classification]`.",
+        )
+        self.auto_required: bool = _get_optional_value(
+            auto_required,
+            _is_auto_available,
+            "etna[auto] is not available, to install it, run `pip install etna[auto]`.",
         )
 
     @staticmethod
     def parse() -> "Settings":
         """Parse and return the settings.
 
         Returns
```

### Comparing `etna-2.0.0/etna/transforms/__init__.py` & `etna-2.1.0/etna/transforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from etna.transforms.feature_selection import FilterFeaturesTransform
 from etna.transforms.feature_selection import GaleShapleyFeatureSelectionTransform
 from etna.transforms.feature_selection import MRMRFeatureSelectionTransform
 from etna.transforms.feature_selection import TreeFeatureSelectionTransform
 from etna.transforms.math import AddConstTransform
 from etna.transforms.math import BoxCoxTransform
 from etna.transforms.math import DifferencingTransform
+from etna.transforms.math import ExogShiftTransform
 from etna.transforms.math import LagTransform
 from etna.transforms.math import LambdaTransform
 from etna.transforms.math import LogTransform
 from etna.transforms.math import MADTransform
 from etna.transforms.math import MaxAbsScalerTransform
 from etna.transforms.math import MaxTransform
 from etna.transforms.math import MeanTransform
```

### Comparing `etna-2.0.0/etna/transforms/base.py` & `etna-2.1.0/etna/transforms/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from typing import Optional
 from typing import Set
 from typing import Union
 
 import pandas as pd
 from typing_extensions import Literal
 
-from etna.core import AbstractSaveable
 from etna.core import BaseMixin
 from etna.core import SaveMixin
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
 from etna.transforms.utils import match_target_quantiles
 
 
 class FutureMixin:
     """Mixin for transforms that can convert non-regressor column to a regressor one."""
 
 
-class Transform(SaveMixin, AbstractSaveable, BaseMixin):
+class Transform(SaveMixin, BaseMixin):
     """Base class to create any transforms to apply to data."""
 
     def __init__(self, required_features: Union[Literal["all"], List[str]]):
         self.required_features = required_features
 
     @abstractmethod
     def get_regressors_info(self) -> List[str]:
@@ -158,14 +158,26 @@
         Returns
         -------
         :
             TSDataset after applying inverse transformation.
         """
         pass
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get grid for tuning hyperparameters.
+
+        This is default implementation with empty grid.
+
+        Returns
+        -------
+        :
+            Empty grid.
+        """
+        return {}
+
 
 class IrreversibleTransform(Transform):
     """Base class to create irreversible transforms."""
 
     def __init__(self, required_features: Union[Literal["all"], List[str]]):
         super().__init__(required_features=required_features)
```

### Comparing `etna-2.0.0/etna/transforms/decomposition/__init__.py` & `etna-2.1.0/etna/transforms/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/__init__.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/base.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from etna.core import BaseMixin
 
 
 class PerIntervalModel(BaseMixin, ABC):
     """Class to handle intervals in change point based transforms.
 
     PerIntervalModel is a class to process intervals between change points
-    in `~etna.transforms.decomposition.change_points_based` transforms.
+    in :py:mod:`~etna.transforms.decomposition.change_points_based` transforms.
     """
 
     @abstractmethod
     def fit(self, features: np.ndarray, target: np.ndarray, *args, **kwargs) -> "PerIntervalModel":
         """Fit per interval model with given params."""
         pass
```

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py` & `etna-2.1.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/decomposition/detrend.py` & `etna-2.1.0/etna/transforms/decomposition/detrend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from typing import Dict
 from typing import List
 
 import numpy as np
 import pandas as pd
 from sklearn.base import RegressorMixin
 from sklearn.linear_model import LinearRegression
 from sklearn.linear_model import TheilSenRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
+from etna.distributions import BaseDistribution
+from etna.distributions import IntDistribution
 from etna.transforms.base import OneSegmentTransform
 from etna.transforms.base import ReversiblePerSegmentWrapper
 from etna.transforms.utils import match_target_quantiles
 
 
 class _OneSegmentLinearTrendBaseTransform(OneSegmentTransform):
-    """LinearTrendBaseTransform is a base class that implements trend subtraction and reconstruction feature."""
+    """Transform for one segment that implements trend subtraction and reconstruction feature."""
 
     def __init__(self, in_column: str, regressor: RegressorMixin, poly_degree: int = 1):
         """
         Create instance of _OneSegmentLinearTrendBaseTransform.
 
         Parameters
         ----------
@@ -133,16 +136,18 @@
             quantiles = match_target_quantiles(set(result.columns))
             for quantile_column_nm in quantiles:
                 result.loc[:, quantile_column_nm] += trend
         return result
 
 
 class LinearTrendTransform(ReversiblePerSegmentWrapper):
-    """
-    Transform that uses :py:class:`sklearn.linear_model.LinearRegression` to find linear or polynomial trend in data.
+    """Transform that uses linear regression with polynomial features to make a detrending.
+
+    Transform fits a :py:class:`sklearn.linear_model.LinearRegression` with polynomial features on each segment.
+    Values predicted by the model are subtracted from each segment.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
     """
 
@@ -170,18 +175,34 @@
             required_features=[self.in_column],
         )
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         return []
 
+    def params_to_tune(self) -> Dict[str, "BaseDistribution"]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes only ``poly_degree`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "poly_degree": IntDistribution(low=1, high=2),
+        }
+
 
 class TheilSenTrendTransform(ReversiblePerSegmentWrapper):
-    """
-    Transform that uses :py:class:`sklearn.linear_model.TheilSenRegressor` to find linear or polynomial trend in data.
+    """Transform that uses Theil–Sen regression with polynomial features to make a detrending.
+
+    Transform fits a :py:class:`sklearn.linear_model.TheilSenRegressor` with polynomial features on each segment.
+    Values predicted by the model are subtracted from each segment.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
 
     Notes
@@ -213,7 +234,21 @@
             ),
             required_features=[self.in_column],
         )
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         return []
+
+    def params_to_tune(self) -> Dict[str, "BaseDistribution"]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``poly_degree`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "poly_degree": IntDistribution(low=1, high=2),
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `etna-2.0.0/etna/transforms/decomposition/stl.py` & `etna-2.1.0/etna/transforms/decomposition/stl.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import pandas as pd
 from statsmodels.tsa.arima.model import ARIMA
 from statsmodels.tsa.base.tsa_model import TimeSeriesModel
 from statsmodels.tsa.exponential_smoothing.ets import ETSModel
 from statsmodels.tsa.forecasting.stl import STLForecast
 from statsmodels.tsa.forecasting.stl import STLForecastResults
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.base import OneSegmentTransform
 from etna.transforms.base import ReversiblePerSegmentWrapper
 from etna.transforms.utils import match_target_quantiles
 
 
 class _OneSegmentSTLTransform(OneSegmentTransform):
     def __init__(
@@ -220,7 +222,22 @@
             ),
             required_features=[self.in_column],
         )
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         return []
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``model``, ``robust``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "model": CategoricalDistribution(["arima", "holt"]),
+            "robust": CategoricalDistribution([False, True]),
+        }
```

### Comparing `etna-2.0.0/etna/transforms/encoders/categorical.py` & `etna-2.1.0/etna/transforms/encoders/categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from enum import Enum
+from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from sklearn.utils._encode import _check_unknown
 from sklearn.utils._encode import _encode
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.base import IrreversibleTransform
 
 
 class ImputerMode(str, Enum):
     """Enum for different imputation strategy."""
 
     new_value = "new_value"
@@ -126,14 +129,28 @@
 
     def _get_column_name(self) -> str:
         """Get the ``out_column`` depending on the transform's parameters."""
         if self.out_column:
             return self.out_column
         return self.__repr__()
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``strategy`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "strategy": CategoricalDistribution(["new_value", "mean"]),
+        }
+
 
 class OneHotEncoderTransform(IrreversibleTransform):
     """Encode categorical feature as a one-hot numeric features.
 
     If unknown category is encountered during transform, the resulting one-hot
     encoded columns for this feature will be all zeros.
     """
```

### Comparing `etna-2.0.0/etna/transforms/encoders/mean_segment_encoder.py` & `etna-2.1.0/etna/transforms/encoders/mean_segment_encoder.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/encoders/segment_encoder.py` & `etna-2.1.0/etna/transforms/encoders/segment_encoder.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/feature_selection/base.py` & `etna-2.1.0/etna/transforms/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/feature_selection/feature_importance.py` & `etna-2.1.0/etna/transforms/feature_selection/feature_importance.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from sklearn.tree import ExtraTreeRegressor
 from typing_extensions import Literal
 
 from etna.analysis import RelevanceTable
 from etna.analysis.feature_selection.mrmr_selection import AggregationMode
 from etna.analysis.feature_selection.mrmr_selection import mrmr
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
+from etna.distributions import IntDistribution
 from etna.transforms.feature_selection import BaseFeatureSelectionTransform
 
 TreeBasedRegressor = Union[
     DecisionTreeRegressor,
     ExtraTreeRegressor,
     RandomForestRegressor,
     ExtraTreesRegressor,
@@ -37,52 +40,75 @@
     -----
     Transform works with any type of features, however most of the models works only with regressors.
     Therefore, it is recommended to pass the regressors into the feature selection transforms.
     """
 
     def __init__(
         self,
-        model: TreeBasedRegressor,
+        model: Union[Literal["catboost"], Literal["random_forest"], TreeBasedRegressor],
         top_k: int,
         features_to_use: Union[List[str], Literal["all"]] = "all",
         return_features: bool = False,
     ):
         """
         Init TreeFeatureSelectionTransform.
 
         Parameters
         ----------
         model:
-            model to make selection, it should have ``feature_importances_`` property
-            (e.g. all tree-based regressors in sklearn)
+            Model to make selection, it should have ``feature_importances_`` property
+            (e.g. all tree-based regressors in sklearn).
+
+            If ``catboost.CatBoostRegressor`` is given with no ``cat_features`` parameter,
+            then ``cat_features`` are set during ``fit`` to be equal to columns of category type.
+
+            Pre-defined options are also available:
+
+            * catboost: ``catboost.CatBoostRegressor(iterations=1000, silent=True)``;
+
+            * random_forest: ``sklearn.ensemble.RandomForestRegressor(n_estimators=100, random_state=0)``.
+
         top_k:
             num of features to select; if there are not enough features, then all will be selected
         features_to_use:
             columns of the dataset to select from; if "all" value is given, all columns are used
         return_features:
             indicates whether to return features or not.
         """
         if not isinstance(top_k, int) or top_k < 0:
             raise ValueError("Parameter top_k should be positive integer")
         super().__init__(features_to_use=features_to_use, return_features=return_features)
-        self.model = model
         self.top_k = top_k
+        if isinstance(model, str):
+            if model == "catboost":
+                self.model = CatBoostRegressor(iterations=1000, silent=True)
+            elif model == "random_forest":
+                self.model = RandomForestRegressor(random_state=0)
+            else:
+                raise ValueError(f"Not a valid option for model: {model}")
+        else:
+            self.model = model
 
     def _get_train(self, df: pd.DataFrame) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """Get train data for model."""
         features = self._get_features_to_use(df)
         df = TSDataset.to_flatten(df).dropna()
         train_target = df["target"]
         train_data = df[features]
         return train_data, train_target
 
     def _get_features_weights(self, df: pd.DataFrame) -> Dict[str, float]:
         """Get weights for features based on model feature importances."""
         train_data, train_target = self._get_train(df)
-        self.model.fit(train_data, train_target)
+        if isinstance(self.model, CatBoostRegressor) and self.model.get_param("cat_features") is None:
+            dtypes = train_data.dtypes
+            cat_features = dtypes[dtypes == "category"].index.tolist()
+            self.model.fit(train_data, train_target, cat_features=cat_features)
+        else:
+            self.model.fit(train_data, train_target)
         weights_array = self.model.feature_importances_
         weights_dict = {column: weights_array[i] for i, column in enumerate(train_data.columns)}
         return weights_dict
 
     @staticmethod
     def _select_top_k_features(weights: Dict[str, float], top_k: int) -> List[str]:
         keys = np.array(list(weights.keys()))
@@ -98,24 +124,42 @@
         Parameters
         ----------
         df:
             dataframe with all segments data
 
         Returns
         -------
-        result: TreeFeatureSelectionTransform
+        result:
             instance after fitting
         """
         if len(self._get_features_to_use(df)) == 0:
             warnings.warn("It is not possible to select features if there aren't any")
             return self
         weights = self._get_features_weights(df)
         self.selected_features = self._select_top_k_features(weights, self.top_k)
         return self
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``model``, ``top_k``. Other parameters are expected to be set by the user.
+
+        For ``model`` parameter only pre-defined options are suggested.
+        For ``top_k`` parameter the maximum suggested value is not greater than ``self.top_k``.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "model": CategoricalDistribution(["catboost", "random_forest"]),
+            "top_k": IntDistribution(low=1, high=self.top_k),
+        }
+
 
 class MRMRFeatureSelectionTransform(BaseFeatureSelectionTransform):
     """Transform that selects features according to MRMR variable selection method adapted to the timeseries case.
 
     Notes
     -----
     Transform works with any type of features, however most of the models works only with regressors.
@@ -123,14 +167,15 @@
     """
 
     def __init__(
         self,
         relevance_table: RelevanceTable,
         top_k: int,
         features_to_use: Union[List[str], Literal["all"]] = "all",
+        fast_redundancy: bool = False,
         relevance_aggregation_mode: str = AggregationMode.mean,
         redundancy_aggregation_mode: str = AggregationMode.mean,
         atol: float = 1e-10,
         return_features: bool = False,
         **relevance_params,
     ):
         """
@@ -141,14 +186,17 @@
         relevance_table:
             method to calculate relevance table
         top_k:
             num of features to select; if there are not enough features, then all will be selected
         features_to_use:
             columns of the dataset to select from
             if "all" value is given, all columns are used
+        fast_redundancy:
+            * True: compute redundancy only inside the the segments, time complexity :math:`O(top\_k * n\_segments * n\_features * history\_len)
+            * False: compute redundancy for all the pairs of segments, time complexity :math:`O(top\_k * n\_segments^2 * n\_features * history\_len)`
         relevance_aggregation_mode:
             the method for relevance values per-segment aggregation
         redundancy_aggregation_mode:
             the method for redundancy values per-segment aggregation
         atol:
             the absolute tolerance to compare the float values
         return_features:
@@ -156,14 +204,15 @@
         """
         if not isinstance(top_k, int) or top_k < 0:
             raise ValueError("Parameter top_k should be positive integer")
 
         super().__init__(features_to_use=features_to_use, return_features=return_features)
         self.relevance_table = relevance_table
         self.top_k = top_k
+        self.fast_redundancy = fast_redundancy
         self.relevance_aggregation_mode = relevance_aggregation_mode
         self.redundancy_aggregation_mode = redundancy_aggregation_mode
         self.atol = atol
         self.relevance_params = relevance_params
 
     def _fit(self, df: pd.DataFrame) -> "MRMRFeatureSelectionTransform":
         """
@@ -172,24 +221,41 @@
         Parameters
         ----------
         df:
             dataframe with all segments data
 
         Returns
         -------
-        result: MRMRFeatureSelectionTransform
+        result:
             instance after fitting
         """
         features = self._get_features_to_use(df)
         ts = TSDataset(df=df, freq=pd.infer_freq(df.index))
         relevance_table = self.relevance_table(ts[:, :, "target"], ts[:, :, features], **self.relevance_params)
         if not self.relevance_table.greater_is_better:
             relevance_table *= -1
         self.selected_features = mrmr(
             relevance_table=relevance_table,
             regressors=ts[:, :, features],
             top_k=self.top_k,
+            fast_redundancy=self.fast_redundancy,
             relevance_aggregation_mode=self.relevance_aggregation_mode,
             redundancy_aggregation_mode=self.redundancy_aggregation_mode,
             atol=self.atol,
         )
         return self
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``top_k`` parameter. Other parameters are expected to be set by the user.
+
+        For ``top_k`` parameter the maximum suggested value is not greater than ``self.top_k``.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "top_k": IntDistribution(low=1, high=self.top_k),
+        }
```

### Comparing `etna-2.0.0/etna/transforms/feature_selection/filter.py` & `etna-2.1.0/etna/transforms/feature_selection/filter.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/feature_selection/gale_shapley.py` & `etna-2.1.0/etna/transforms/feature_selection/gale_shapley.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from typing import Union
 
 import pandas as pd
 from typing_extensions import Literal
 
 from etna.analysis import RelevanceTable
 from etna.core import BaseMixin
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
+from etna.distributions import IntDistribution
 from etna.transforms.feature_selection.base import BaseFeatureSelectionTransform
 
 
 class BaseGaleShapley(BaseMixin):
     """Base class for a member of Gale-Shapley matching."""
 
     def __init__(self, name: str, ranked_candidates: List[str]):
@@ -381,7 +384,24 @@
             else:
                 selected_features = list(matches.values())
             self.selected_features.extend(selected_features)
             segment_features_ranking = self._update_ranking_list(
                 segment_features_ranking=segment_features_ranking, features_to_drop=selected_features
             )
         return self
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``top_k``, ``use_rank``. Other parameters are expected to be set by the user.
+
+        For ``top_k`` parameter the maximum suggested value is not greater than ``self.top_k``.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "top_k": IntDistribution(low=1, high=self.top_k),
+            "use_rank": CategoricalDistribution([False, True]),
+        }
```

### Comparing `etna-2.0.0/etna/transforms/math/__init__.py` & `etna-2.1.0/etna/transforms/math/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from etna.transforms.math.add_constant import AddConstTransform
 from etna.transforms.math.apply_lambda import LambdaTransform
 from etna.transforms.math.differencing import DifferencingTransform
+from etna.transforms.math.lags import ExogShiftTransform
 from etna.transforms.math.lags import LagTransform
 from etna.transforms.math.log import LogTransform
 from etna.transforms.math.power import BoxCoxTransform
 from etna.transforms.math.power import YeoJohnsonTransform
 from etna.transforms.math.scalers import MaxAbsScalerTransform
 from etna.transforms.math.scalers import MinMaxScalerTransform
 from etna.transforms.math.scalers import RobustScalerTransform
```

### Comparing `etna-2.0.0/etna/transforms/math/add_constant.py` & `etna-2.1.0/etna/transforms/math/add_constant.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/math/apply_lambda.py` & `etna-2.1.0/etna/transforms/math/apply_lambda.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/math/differencing.py` & `etna-2.1.0/etna/transforms/math/differencing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from typing import Union
 from typing import cast
 
 import numpy as np
 import pandas as pd
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import IntDistribution
 from etna.transforms.base import ReversibleTransform
 from etna.transforms.utils import check_new_segments
 from etna.transforms.utils import match_target_quantiles
 
 
 class _SingleDifferencingTransform(ReversibleTransform):
     """Calculate a time series differences of order 1.
@@ -469,7 +471,21 @@
         segments = df.columns.get_level_values("segment").unique().tolist()
         check_new_segments(transform_segments=segments, fit_segments=self._fit_segments)
 
         result_df = df
         for transform in self._differencing_transforms[::-1]:
             result_df = transform._inverse_transform(result_df)
         return result_df
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``order`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "order": IntDistribution(low=1, high=2),
+        }
```

### Comparing `etna-2.0.0/etna/transforms/math/lags.py` & `etna-2.1.0/etna/transforms/timestamp/holiday.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,89 @@
+import datetime
 from typing import List
 from typing import Optional
-from typing import Union
 
+import holidays
+import numpy as np
 import pandas as pd
 
 from etna.transforms.base import FutureMixin
 from etna.transforms.base import IrreversibleTransform
 
 
-class LagTransform(IrreversibleTransform, FutureMixin):
-    """Generates series of lags from given dataframe."""
+class HolidayTransform(IrreversibleTransform, FutureMixin):
+    """HolidayTransform generates series that indicates holidays in given dataframe."""
 
-    def __init__(self, in_column: str, lags: Union[List[int], int], out_column: Optional[str] = None):
-        """Create instance of LagTransform.
+    def __init__(self, iso_code: str = "RUS", out_column: Optional[str] = None):
+        """
+        Create instance of HolidayTransform.
 
         Parameters
         ----------
-        in_column:
-            name of processed column
-        lags:
-            int value or list of values for lags computation; if int, generate range of lags from 1 to given value
+        iso_code:
+            internationally recognised codes, designated to country for which we want to find the holidays
         out_column:
-            base for the name of created columns;
-
-            * if set the final name is '{out_column}_{lag_number}';
-
-            * if don't set, name will be ``transform.__repr__()``,
-              repr will be made for transform that creates exactly this column
-
-        Raises
-        ------
-        ValueError:
-            if lags value contains non-positive values
-        """
-        super().__init__(required_features=[in_column])
-        if isinstance(lags, int):
-            if lags < 1:
-                raise ValueError(f"{type(self).__name__} works only with positive lags values, {lags} given")
-            self.lags = list(range(1, lags + 1))
-        else:
-            if any(lag_value < 1 for lag_value in lags):
-                raise ValueError(f"{type(self).__name__} works only with positive lags values")
-            self.lags = lags
-
-        self.in_column = in_column
+            name of added column. Use ``self.__repr__()`` if not given.
+        """
+        super().__init__(required_features=["target"])
+        self.iso_code = iso_code
+        self.holidays = holidays.CountryHoliday(iso_code)
         self.out_column = out_column
 
-    def _get_column_name(self, lag: int) -> str:
-        if self.out_column is None:
-            temp_transform = LagTransform(in_column=self.in_column, out_column=self.out_column, lags=[lag])
-            return repr(temp_transform)
+    def _get_column_name(self) -> str:
+        if self.out_column:
+            return self.out_column
         else:
-            return f"{self.out_column}_{lag}"
+            return self.__repr__()
 
-    def _fit(self, df: pd.DataFrame) -> "LagTransform":
-        """Fit method does nothing and is kept for compatibility.
+    def _fit(self, df: pd.DataFrame) -> "HolidayTransform":
+        """
+        Fit HolidayTransform with data from df. Does nothing in this case.
 
         Parameters
         ----------
-        df:
-            dataframe with data.
-
-        Returns
-        -------
-        result: LagTransform
+        df: pd.DataFrame
+            value series with index column in timestamp format
         """
         return self
 
     def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Add lags to the dataset.
+        """
+        Transform data from df with HolidayTransform and generate a column of holidays flags.
 
         Parameters
         ----------
-        df:
-            dataframe with data to transform.
+        df: pd.DataFrame
+            value series with index column in timestamp format
 
         Returns
         -------
-        result: pd.Dataframe
-            transformed dataframe
+        :
+            pd.DataFrame with added holidays
         """
-        result = df
-        segments = sorted(set(df.columns.get_level_values("segment")))
-        all_transformed_features = []
-        features = df.loc[:, pd.IndexSlice[:, self.in_column]]
-        for lag in self.lags:
-            column_name = self._get_column_name(lag)
-            transformed_features = features.shift(lag)
-            transformed_features.columns = pd.MultiIndex.from_product([segments, [column_name]])
-            all_transformed_features.append(transformed_features)
-        result = pd.concat([result] + all_transformed_features, axis=1)
-        result = result.sort_index(axis=1)
-        return result
+        if (df.index[1] - df.index[0]) > datetime.timedelta(days=1):
+            raise ValueError("Frequency of data should be no more than daily.")
+
+        cols = df.columns.get_level_values("segment").unique()
+
+        out_column = self._get_column_name()
+        encoded_matrix = np.array([int(x in self.holidays) for x in df.index])
+        encoded_matrix = encoded_matrix.reshape(-1, 1).repeat(len(cols), axis=1)
+        encoded_df = pd.DataFrame(
+            encoded_matrix,
+            columns=pd.MultiIndex.from_product([cols, [out_column]], names=("segment", "feature")),
+            index=df.index,
+        )
+        encoded_df = encoded_df.astype("category")
+
+        df = df.join(encoded_df)
+        df = df.sort_index(axis=1)
+        return df
 
     def get_regressors_info(self) -> List[str]:
-        """Return the list with regressors created by the transform."""
-        return [self._get_column_name(lag) for lag in self.lags]
+        """Return the list with regressors created by the transform.
+        Returns
+        -------
+        :
+            List with regressors created by the transform.
+        """
+        return [self._get_column_name()]
```

### Comparing `etna-2.0.0/etna/transforms/math/log.py` & `etna-2.1.0/etna/transforms/math/log.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/math/power.py` & `etna-2.1.0/etna/transforms/math/power.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from sklearn.preprocessing import PowerTransformer
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.math.sklearn import SklearnTransform
 from etna.transforms.math.sklearn import TransformMode
 
 
 class YeoJohnsonTransform(SklearnTransform):
     """YeoJohnsonTransform applies Yeo-Johns transformation to a DataFrame.
 
@@ -54,14 +57,32 @@
             in_column=in_column,
             inplace=inplace,
             out_column=out_column,
             transformer=PowerTransformer(method="yeo-johnson", standardize=self.standardize),
             mode=mode,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``mode``, ``standardize``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "standardize": CategoricalDistribution([False, True]),
+            }
+        )
+        return grid
+
 
 class BoxCoxTransform(SklearnTransform):
     """BoxCoxTransform applies Box-Cox transformation to DataFrame.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
@@ -105,9 +126,27 @@
             in_column=in_column,
             inplace=inplace,
             out_column=out_column,
             transformer=PowerTransformer(method="box-cox", standardize=self.standardize),
             mode=mode,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``mode``, ``standardize``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "standardize": CategoricalDistribution([False, True]),
+            }
+        )
+        return grid
+
 
 __all__ = ["BoxCoxTransform", "YeoJohnsonTransform"]
```

### Comparing `etna-2.0.0/etna/transforms/math/scalers.py` & `etna-2.1.0/etna/transforms/math/scalers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 from sklearn.preprocessing import MaxAbsScaler
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.preprocessing import RobustScaler
 from sklearn.preprocessing import StandardScaler
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.math.sklearn import SklearnTransform
 from etna.transforms.math.sklearn import TransformMode
 
 
 class StandardScalerTransform(SklearnTransform):
     """Standardize features by removing the mean and scaling to unit variance.
 
@@ -65,14 +68,34 @@
             in_column=in_column,
             transformer=StandardScaler(with_mean=self.with_mean, with_std=self.with_std, copy=False),
             out_column=out_column,
             inplace=inplace,
             mode=mode,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``mode``, ``with_mean``, ``with_std``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "with_mean": CategoricalDistribution([False, True]),
+                "with_std": CategoricalDistribution([False, True]),
+            }
+        )
+        return grid
+
 
 class RobustScalerTransform(SklearnTransform):
     """Scale features using statistics that are robust to outliers.
 
     Uses :py:class:`sklearn.preprocessing.RobustScaler` inside.
 
     Warning
@@ -141,14 +164,35 @@
                 quantile_range=self.quantile_range,
                 unit_variance=self.unit_variance,
                 copy=False,
             ),
             mode=mode,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``mode``, ``with_centering``, ``with_scaling``, ``unit_variance``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "with_centering": CategoricalDistribution([False, True]),
+                "with_scaling": CategoricalDistribution([False, True]),
+                "unit_variance": CategoricalDistribution([False, True]),
+            }
+        )
+        return grid
+
 
 class MinMaxScalerTransform(SklearnTransform):
     """Transform features by scaling each feature to a given range.
 
     Uses :py:class:`sklearn.preprocessing.MinMaxScaler` inside.
 
     Warning
@@ -199,14 +243,32 @@
             in_column=in_column,
             inplace=inplace,
             out_column=out_column,
             transformer=MinMaxScaler(feature_range=self.feature_range, clip=self.clip, copy=False),
             mode=mode,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``mode``, ``clip``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "clip": CategoricalDistribution([False, True]),
+            }
+        )
+        return grid
+
 
 class MaxAbsScalerTransform(SklearnTransform):
     """Scale each feature by its maximum absolute value.
 
     Uses :py:class:`sklearn.preprocessing.MaxAbsScaler` inside.
 
     Warning
```

### Comparing `etna-2.0.0/etna/transforms/math/sklearn.py` & `etna-2.1.0/etna/transforms/math/sklearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import numpy as np
 import pandas as pd
 from sklearn.base import TransformerMixin
 
 from etna.core import StringEnumWithRepr
 from etna.datasets import TSDataset
 from etna.datasets import set_columns_wide
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.base import ReversibleTransform
 from etna.transforms.utils import check_new_segments
 from etna.transforms.utils import match_target_quantiles
 
 
 class TransformMode(StringEnumWithRepr):
     """Enum for different metric aggregation modes."""
@@ -294,7 +296,21 @@
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         if self.out_column_regressors is None:
             raise ValueError("Fit the transform to get the correct regressors info!")
         if self.inplace:
             return []
         return self.out_column_regressors
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes ``mode`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "mode": CategoricalDistribution(["per-segment", "macro"]),
+        }
```

### Comparing `etna-2.0.0/etna/transforms/math/statistics.py` & `etna-2.1.0/etna/transforms/math/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from abc import ABC
 from abc import abstractmethod
+from typing import Dict
 from typing import List
 from typing import Optional
 
 import bottleneck as bn
 import numpy as np
 import pandas as pd
 
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
 from etna.transforms.base import IrreversibleTransform
 
 
 class WindowStatisticsTransform(IrreversibleTransform, ABC):
     """WindowStatisticsTransform handles computation of statistical features on windows."""
 
     def __init__(
@@ -108,14 +112,28 @@
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         if self.in_column_regressor is None:
             raise ValueError("Fit the transform to get the correct regressors info!")
         return [self.out_column_name] if self.in_column_regressor else []
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes only ``window`` parameter. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "window": IntDistribution(low=1, high=20),
+        }
+
 
 class MeanTransform(WindowStatisticsTransform):
     """MeanTransform computes average value for given window.
 
     .. math::
        MeanTransform(x_t) = \\sum_{i=1}^{window}{x_{t - i}\\cdot\\alpha^{i - 1}}
     """
@@ -189,14 +207,32 @@
         """Compute weighted average for window series."""
         mean = np.zeros((series.shape[0], series.shape[1]))
         for segment in range(mean.shape[1]):
             # Loop prevents from memory overflow, 3d tensor is materialized after multiplication
             mean[:, segment] = bn.nanmean(series[:, segment] * self._alpha_range, axis=1)
         return mean
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``window``, ``alpha``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "alpha": FloatDistribution(low=0.2, high=1),
+            }
+        )
+        return grid
+
 
 class StdTransform(WindowStatisticsTransform):
     """StdTransform computes std value for given window.
 
     Notes
     -----
     Note that ``pd.Series([1]).std()`` is ``np.nan``.
@@ -305,14 +341,32 @@
 
     def _aggregate(self, series: np.ndarray) -> np.ndarray:
         """Compute quantile over the series."""
         # There is no "nanquantile" in bottleneck, "apply_along_axis" can't be replace with "axis=2"
         series = np.apply_along_axis(np.nanquantile, axis=2, arr=series, q=self.quantile)
         return series
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``window``, ``quantile``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        grid = super().params_to_tune()
+        grid.update(
+            {
+                "quantile": FloatDistribution(low=0, high=1),
+            }
+        )
+        return grid
+
 
 class MinTransform(WindowStatisticsTransform):
     """MinTransform computes min value for given window."""
 
     def __init__(
         self,
         in_column: str,
```

### Comparing `etna-2.0.0/etna/transforms/missing_values/resample.py` & `etna-2.1.0/etna/transforms/missing_values/resample.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,42 +136,46 @@
 
         out_column:
             name of added column. If not given, use ``self.__repr__()``
         """
         self.in_column = in_column
         self.distribution_column = distribution_column
         self.inplace = inplace
-        self.out_column = self._get_out_column(out_column)
+        self.out_column = out_column
         self.in_column_regressor: Optional[bool] = None
+
+        if self.inplace and out_column:
+            warnings.warn("Transformation will be applied inplace, out_column param will be ignored")
+
         super().__init__(
             transform=_OneSegmentResampleWithDistributionTransform(
                 in_column=in_column,
                 distribution_column=distribution_column,
                 inplace=inplace,
-                out_column=self.out_column,
+                out_column=self._get_column_name(),
             ),
             required_features=[in_column, distribution_column],
         )
 
-    def _get_out_column(self, out_column: Optional[str]) -> str:
+    def _get_column_name(
+        self,
+    ) -> str:
         """Get the `out_column` depending on the transform's parameters."""
-        if self.inplace and out_column:
-            warnings.warn("Transformation will be applied inplace, out_column param will be ignored")
         if self.inplace:
             return self.in_column
-        if out_column:
-            return out_column
+        if self.out_column:
+            return self.out_column
         return self.__repr__()
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         if self.in_column_regressor is None:
             raise ValueError("Fit the transform to get the correct regressors info!")
         if self.inplace:
             return []
-        return [self.out_column] if self.in_column_regressor else []
+        return [self._get_column_name()] if self.in_column_regressor else []
 
     def fit(self, ts: TSDataset) -> "ResampleWithDistributionTransform":
         """Fit the transform."""
         self.in_column_regressor = self.in_column in ts.regressors
         super().fit(ts)
         return self
```

### Comparing `etna-2.0.0/etna/transforms/outliers/base.py` & `etna-2.1.0/etna/transforms/outliers/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.0.0/etna/transforms/outliers/point_outliers.py` & `etna-2.1.0/etna/transforms/outliers/point_outliers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import Union
 
 import pandas as pd
+from typing_extensions import Literal
 
 from etna import SETTINGS
 from etna.analysis import absolute_difference_distance
 from etna.analysis import get_anomalies_density
 from etna.analysis import get_anomalies_median
 from etna.analysis import get_anomalies_prediction_interval
 from etna.datasets import TSDataset
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
+from etna.distributions import FloatDistribution
+from etna.distributions import IntDistribution
 from etna.models import SARIMAXModel
 from etna.transforms.outliers.base import OutliersTransform
 
 if SETTINGS.prophet_required:
     from etna.models import ProphetModel
 
 
@@ -55,14 +60,29 @@
         Returns
         -------
         :
             dict of outliers in format {segment: [outliers_timestamps]}
         """
         return get_anomalies_median(ts=ts, in_column=self.in_column, window_size=self.window_size, alpha=self.alpha)
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``window_size``, ``alpha``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "window_size": IntDistribution(low=3, high=30),
+            "alpha": FloatDistribution(low=0.5, high=5),
+        }
+
 
 class DensityOutliersTransform(OutliersTransform):
     """Transform that uses :py:func:`~etna.analysis.outliers.density_outliers.get_anomalies_density` to find anomalies in data.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
@@ -116,22 +136,39 @@
             in_column=self.in_column,
             window_size=self.window_size,
             distance_coef=self.distance_coef,
             n_neighbors=self.n_neighbors,
             distance_func=self.distance_func,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``window_size``, ``distance_coef``, ``n_neighbors``.
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "window_size": IntDistribution(low=3, high=30),
+            "distance_coef": FloatDistribution(low=0.5, high=5),
+            "n_neighbors": IntDistribution(low=1, high=10),
+        }
+
 
 class PredictionIntervalOutliersTransform(OutliersTransform):
     """Transform that uses :py:func:`~etna.analysis.outliers.prediction_interval_outliers.get_anomalies_prediction_interval` to find anomalies in data."""
 
     def __init__(
         self,
         in_column: str,
-        model: Union[Type["ProphetModel"], Type["SARIMAXModel"]],
+        model: Union[Literal["prophet"], Literal["sarimax"], Type["ProphetModel"], Type["SARIMAXModel"]],
         interval_width: float = 0.95,
         **model_kwargs,
     ):
         """Create instance of PredictionIntervalOutliersTransform.
 
         Parameters
         ----------
@@ -145,16 +182,28 @@
         Notes
         -----
         For not "target" column only column data will be used for learning.
         """
         self.model = model
         self.interval_width = interval_width
         self.model_kwargs = model_kwargs
+        self._model_type = self._get_model_type(model)
         super().__init__(in_column=in_column)
 
+    @staticmethod
+    def _get_model_type(
+        model: Union[Literal["prophet"], Literal["sarimax"], Type["ProphetModel"], Type["SARIMAXModel"]]
+    ) -> Union[Type["ProphetModel"], Type["SARIMAXModel"]]:
+        if isinstance(model, str):
+            if model == "prophet":
+                return ProphetModel
+            elif model == "sarimax":
+                return SARIMAXModel
+        return model
+
     def detect_outliers(self, ts: TSDataset) -> Dict[str, List[pd.Timestamp]]:
         """Call :py:func:`~etna.analysis.outliers.prediction_interval_outliers.get_anomalies_prediction_interval` function with self parameters.
 
         Parameters
         ----------
         ts:
             dataset to process
@@ -162,19 +211,34 @@
         Returns
         -------
         :
             dict of outliers in format {segment: [outliers_timestamps]}
         """
         return get_anomalies_prediction_interval(
             ts=ts,
-            model=self.model,
+            model=self._model_type,
             interval_width=self.interval_width,
             in_column=self.in_column,
             **self.model_kwargs,
         )
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``interval_width``, ``model``. Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "interval_width": FloatDistribution(low=0.8, high=1.0),
+            "model": CategoricalDistribution(["prophet", "sarimax"]),
+        }
+
 
 __all__ = [
     "MedianOutliersTransform",
     "DensityOutliersTransform",
     "PredictionIntervalOutliersTransform",
 ]
```

### Comparing `etna-2.0.0/etna/transforms/timestamp/date_flags.py` & `etna-2.1.0/etna/transforms/timestamp/date_flags.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from copy import deepcopy
 from math import ceil
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 
 import numpy as np
 import pandas as pd
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.base import FutureMixin
 from etna.transforms.base import IrreversibleTransform
 
 
 class DateFlagsTransform(IrreversibleTransform, FutureMixin):
     """DateFlagsTransform is a class that implements extraction of the main date-based features from datetime column.
 
@@ -341,9 +344,36 @@
 
     @staticmethod
     def _get_weekends(timestamp_series: pd.Series) -> np.ndarray:
         """Generate an array with the weekends flags."""
         weekend_days = (5, 6)
         return timestamp_series.apply(lambda x: x.weekday() in weekend_days).values
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``day_number_in_week``, ``day_number_in_month``, ``day_number_in_year``,
+        ``week_number_in_month``, ``week_number_in_year``, ``month_number_in_year``, ``season_number``,
+        ``year_number``, ``is_weekend``.
+        Other parameters are expected to be set by the user.
+
+        There are no restrictions on all ``False`` values for the flags.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "day_number_in_week": CategoricalDistribution([False, True]),
+            "day_number_in_month": CategoricalDistribution([False, True]),
+            "day_number_in_year": CategoricalDistribution([False, True]),
+            "week_number_in_month": CategoricalDistribution([False, True]),
+            "week_number_in_year": CategoricalDistribution([False, True]),
+            "month_number_in_year": CategoricalDistribution([False, True]),
+            "season_number": CategoricalDistribution([False, True]),
+            "year_number": CategoricalDistribution([False, True]),
+            "is_weekend": CategoricalDistribution([False, True]),
+        }
+
 
 __all__ = ["DateFlagsTransform"]
```

### Comparing `etna-2.0.0/etna/transforms/timestamp/fourier.py` & `etna-2.1.0/etna/transforms/timestamp/fourier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import math
+from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 
 import numpy as np
 import pandas as pd
 
+from etna.distributions import BaseDistribution
+from etna.distributions import IntDistribution
 from etna.transforms.base import FutureMixin
 from etna.transforms.base import IrreversibleTransform
 
 
 class FourierTransform(IrreversibleTransform, FutureMixin):
     """Adds fourier features to the dataset.
 
@@ -68,39 +71,42 @@
             if order is < 1 or > ceil(period/2)
         ValueError:
             if at least one mod is < 1 or >= period
         """
         if period < 2:
             raise ValueError("Period should be at least 2")
         self.period = period
-        self.mods: Sequence[int]
+
+        self.order = order
+        self.mods = mods
+        self._mods: Sequence[int]
 
         if order is not None and mods is None:
             if order < 1 or order > math.ceil(period / 2):
                 raise ValueError("Order should be within [1, ceil(period/2)] range")
-            self.mods = [mod for mod in range(1, 2 * order + 1) if mod < period]
+            self._mods = [mod for mod in range(1, 2 * order + 1) if mod < period]
         elif mods is not None and order is None:
             if min(mods) < 1 or max(mods) >= period:
                 raise ValueError("Every mod should be within [1, int(period)) range")
-            self.mods = mods
+            self._mods = mods
         else:
             raise ValueError("There should be exactly one option set: order or mods")
-        self.order = None
+
         self.out_column = out_column
         super().__init__(required_features=["target"])
 
     def _get_column_name(self, mod: int) -> str:
         if self.out_column is None:
             return f"{FourierTransform(period=self.period, mods=[mod]).__repr__()}"
         else:
             return f"{self.out_column}_{mod}"
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
-        output_columns = [self._get_column_name(mod=mod) for mod in self.mods]
+        output_columns = [self._get_column_name(mod=mod) for mod in self._mods]
         return output_columns
 
     def _fit(self, df: pd.DataFrame) -> "FourierTransform":
         """Fit method does nothing and is kept for compatibility.
 
         Parameters
         ----------
@@ -139,14 +145,31 @@
         -------
         result: pd.Dataframe
             transformed dataframe
         """
         features = pd.DataFrame(index=df.index)
         elapsed = np.arange(features.shape[0]) / self.period
 
-        for mod in self.mods:
+        for mod in self._mods:
             order = (mod + 1) // 2
             is_cos = mod % 2 == 0
 
             features[self._get_column_name(mod)] = np.sin(2 * np.pi * order * elapsed + np.pi / 2 * is_cos)
 
         return self._construct_answer(df, features)
+
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        If ``self.order`` is set then this grid tunes ``order`` parameter:
+        Other parameters are expected to be set by the user.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        if self.mods is not None:
+            return {}
+
+        max_value = math.ceil(self.period / 2)
+        return {"order": IntDistribution(low=1, high=max_value, log=True)}
```

### Comparing `etna-2.0.0/etna/transforms/timestamp/special_days.py` & `etna-2.1.0/etna/transforms/timestamp/special_days.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import pandas as pd
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.base import FutureMixin
 from etna.transforms.base import IrreversiblePerSegmentWrapper
 from etna.transforms.base import OneSegmentTransform
 
 
 def calc_day_number_in_week(datetime_day: datetime.datetime) -> int:
     return datetime_day.weekday()
@@ -212,9 +214,27 @@
         output_columns = []
         if self.find_special_weekday:
             output_columns.append("anomaly_weekdays")
         if self.find_special_month_day:
             output_columns.append("anomaly_monthdays")
         return output_columns
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``find_special_weekday``, ``find_special_month_day``.
+        Other parameters are expected to be set by the user.
+
+        There are no restrictions on all ``False`` values for the flags.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "find_special_weekday": CategoricalDistribution([False, True]),
+            "find_special_month_day": CategoricalDistribution([False, True]),
+        }
+
 
 __all__ = ["SpecialDaysTransform"]
```

### Comparing `etna-2.0.0/etna/transforms/timestamp/time_flags.py` & `etna-2.1.0/etna/transforms/timestamp/time_flags.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from copy import deepcopy
+from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
+from etna.distributions import BaseDistribution
+from etna.distributions import CategoricalDistribution
 from etna.transforms.base import FutureMixin
 from etna.transforms.base import IrreversibleTransform
 
 
 class TimeFlagsTransform(IrreversibleTransform, FutureMixin):
     """TimeFlagsTransform is a class that implements extraction of the main time-based features from datetime column."""
 
@@ -198,9 +201,32 @@
     def _get_period_in_day(timestamp_series: pd.Series, period_in_hours: int = 12) -> np.ndarray:
         """Generate an array with the period number in the day.
 
         Accepts a period length in hours as input and returns array where timestamps marked by period number.
         """
         return timestamp_series.apply(lambda x: x.hour // period_in_hours).values
 
+    def params_to_tune(self) -> Dict[str, BaseDistribution]:
+        """Get default grid for tuning hyperparameters.
+
+        This grid tunes parameters: ``minute_in_hour_number``, ``fifteen_minutes_in_hour_number``, ``hour_number``,
+        ``half_hour_number``, ``half_day_number``, ``one_third_day_number``.
+        Other parameters are expected to be set by the user.
+
+        There are no restrictions on all ``False`` values for the flags.
+
+        Returns
+        -------
+        :
+            Grid to tune.
+        """
+        return {
+            "minute_in_hour_number": CategoricalDistribution([False, True]),
+            "fifteen_minutes_in_hour_number": CategoricalDistribution([False, True]),
+            "hour_number": CategoricalDistribution([False, True]),
+            "half_hour_number": CategoricalDistribution([False, True]),
+            "half_day_number": CategoricalDistribution([False, True]),
+            "one_third_day_number": CategoricalDistribution([False, True]),
+        }
+
 
 __all__ = ["TimeFlagsTransform"]
```

### Comparing `etna-2.0.0/etna/transforms/utils.py` & `etna-2.1.0/etna/transforms/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import reprlib
-from typing import List
+from typing import Iterable
 from typing import Optional
 
 from etna.datasets.utils import inverse_transform_target_components  # noqa: F401
 from etna.datasets.utils import match_target_quantiles  # noqa: F401
 
 
-def check_new_segments(transform_segments: List[str], fit_segments: Optional[List[str]]):
+def check_new_segments(transform_segments: Iterable[str], fit_segments: Optional[Iterable[str]]):
     """Check if there are any new segments that weren't present during training."""
     if fit_segments is None:
         raise ValueError("Transform is not fitted!")
 
     new_segments = set(transform_segments) - set(fit_segments)
     if len(new_segments) > 0:
         raise NotImplementedError(
```

### Comparing `etna-2.0.0/pyproject.toml` & `etna-2.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "etna"
-version = "2.0.0"
+version = "2.1.0"
 repository = "https://github.com/tinkoff-ai/etna"
 readme = "README.md"
 description = "ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun."
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -41,29 +41,29 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.11.0"
 scikit-learn = ">=0.24, <2"
 pandas = "^1.1"
 catboost = ">=0.21"
-ruptures = "1.1.5"
+ruptures = "^1.1.5"
 numba = ">=0.53.1,<0.56.0"
 seaborn = "^0.11.1"
 statsmodels = ">=0.12,<0.14"
 pmdarima = ">=1.8.0"
 dill = "^0.3.4"
 toml = "^0.10.2"
 loguru = "^0.5.3"
 hydra-slayer = "^0.2.0"
 typer = "^0.4.0"
 omegaconf = "^2.1.1"
-holidays = "^0.13"
+holidays = ">=0.13,<1.0"
 boto3 = "^1.5"
 botocore = "*"
-scipy = "<1.8.0"
+scipy = "^1.0"
 Bottleneck = "^1.3.4"
 numpy = "*"
 joblib = "*"
 plotly = "*"
 hydra_slayer = "*"
 matplotlib = "*"
 typing_extensions = "*"
@@ -76,14 +76,15 @@
 torch = {version = ">=1.8.0,<1.12.0", optional = true}
 pytorch-forecasting = {version = "^0.9.0", optional = true}
 pytorch-lightning = {version = "*", optional = true}
 
 wandb = {version = "^0.12.2", optional = true}
 
 optuna = {version = ">=2.5.0,<3.0.0", optional = true}
+sqlalchemy = {version = "^1.1.0", optional = true}
 
 sphinx-mathjax-offline = {version = "^0.0.1", optional = true}
 nbsphinx = {version = "^0.8.2", optional = true}
 Sphinx = {version = "^4.1", optional = true}
 numpydoc = {version = "^1.1.0", optional = true}
 sphinx-rtd-theme = {version = "^0.5.1", optional = true}
 myst-parser = {version = "^0.15.0", optional = true}
@@ -96,62 +97,63 @@
 black = {extras = ["jupyter"], version = "^22.3.0", optional = true}
 isort = {version = "^5.8.0", optional = true}
 flake8 = {version = "^3.9.2", optional = true}
 pep8-naming = {version = "^0.12.1", optional = true}
 flake8-bugbear = {version = "^22.4.25", optional = true}
 flake8-comprehensions = {version = "^3.9.0", optional = true}
 flake8-docstrings = {version = "^1.6.0", optional = true}
-mypy = {version = "^0.950", optional = true}
+mypy = {version = ">=0.950,<2", optional = true}
 types-PyYAML = {version = "^6.0.0", optional = true}
 codespell = {version = "^2.0.0", optional = true}
 
 click = {version = ">=8.0.1, <8.1", optional = true}
 semver = {version = "^2.13.0", optional = true}
 ipywidgets = {version = "^7.6.5", optional = true}
 
 jupyter = {version = "*", optional = true}
 nbconvert = {version = "*", optional = true}
 pyts = {version = "^0.12.0", optional = true}
+tsfresh = {version = "~0.20.0", optional = true}
 types-setuptools = {version = "^65.7.0", optional = true}
 
 
 [tool.poetry.extras]
 # optional deps
 prophet = ["prophet"]
 torch = ["torch", "pytorch-forecasting", "pytorch-lightning"]
 wandb = ["wandb"]
-auto = ["optuna"]
-classification = ["pyts"]
+auto = ["optuna", "sqlalchemy"]
+classification = ["pyts", "tsfresh"]
 # dev deps
 release = ["click", "semver"]
 docs = ["Sphinx", "numpydoc", "sphinx-rtd-theme", "nbsphinx", "sphinx-mathjax-offline", "myst-parser", "GitPython"]
 tests = ["pytest-cov", "coverage", "pytest"]
 jupyter = ["jupyter", "nbconvert", "black"]
 style = ["black", "isort", "flake8", "pep8-naming", "flake8-docstrings", "mypy", "types-PyYAML", "codespell", "flake8-bugbear", "flake8-comprehensions", "types-setuptools"]
 
 all = [
     "prophet",
-    "torch", "pytorch-forecasting",
+    "torch", "pytorch-forecasting", "pytorch-lightning",
     "wandb",
-    "optuna",
-    "pyts"
+    "optuna", "sqlalchemy",
+    "pyts", "tsfresh"
 ]
 
 all-dev = [
     "prophet",
-    "torch", "pytorch-forecasting",
+    "torch", "pytorch-forecasting", "pytorch-lightning",
     "wandb",
-    "optuna",
+    "optuna", "sqlalchemy",
     "click", "semver",
     "Sphinx", "numpydoc", "sphinx-rtd-theme", "nbsphinx", "sphinx-mathjax-offline", "myst-parser", "GitPython",
     "pytest-cov", "coverage", "pytest",
     "black", "isort", "flake8", "pep8-naming", "flake8-docstrings", "mypy", "types-PyYAML", "codespell", "flake8-bugbear", "flake8-comprehensions", "types-setuptools",
     "click", "semver",
     "jupyter", "nbconvert",
-    "pyts"
+    "pyts", "tsfresh"
 ]
 
 [tool.poetry.scripts]
 etna = "etna.commands.__main__:app"
 
 [tool.black]
 line-length = 120
```

### Comparing `etna-2.0.0/PKG-INFO` & `etna-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etna
-Version: 2.0.0
+Version: 2.1.0
 Summary: ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun.
 Home-page: https://github.com/tinkoff-ai/etna
 License: Apache-2.0
 Author: Andrey Alekseev
 Author-email: ilekseev@gmail.com
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,18 +15,14 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: all-dev
 Provides-Extra: auto
 Provides-Extra: classification
 Provides-Extra: docs
@@ -49,24 +45,24 @@
 Requires-Dist: codespell (>=2.0.0,<3.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: coverage (>=5.4,<6.0) ; extra == "tests" or extra == "all-dev"
 Requires-Dist: dill (>=0.3.4,<0.4.0)
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: flake8-bugbear (>=22.4.25,<23.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: flake8-comprehensions (>=3.9.0,<4.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "style" or extra == "all-dev"
-Requires-Dist: holidays (>=0.13,<0.14)
+Requires-Dist: holidays (>=0.13,<1.0)
 Requires-Dist: hydra-slayer (>=0.2.0,<0.3.0)
 Requires-Dist: hydra_slayer
 Requires-Dist: ipywidgets (>=7.6.5,<8.0.0)
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: joblib
 Requires-Dist: jupyter ; extra == "jupyter" or extra == "all-dev"
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: matplotlib
-Requires-Dist: mypy (>=0.950,<0.951) ; extra == "style" or extra == "all-dev"
+Requires-Dist: mypy (>=0.950,<2) ; extra == "style" or extra == "all-dev"
 Requires-Dist: myst-parser (>=0.15.0,<0.16.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: nbconvert ; extra == "jupyter" or extra == "all-dev"
 Requires-Dist: nbsphinx (>=0.8.2,<0.9.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: numba (>=0.53.1,<0.56.0)
 Requires-Dist: numpy
 Requires-Dist: numpydoc (>=1.1.0,<2.0.0) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: omegaconf (>=2.1.1,<3.0.0)
@@ -75,27 +71,29 @@
 Requires-Dist: pep8-naming (>=0.12.1,<0.13.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: plotly
 Requires-Dist: pmdarima (>=1.8.0)
 Requires-Dist: prophet (>=1.0,<2.0) ; extra == "prophet" or extra == "all" or extra == "all-dev"
 Requires-Dist: pytest (>=6.2,<7.0) ; extra == "tests" or extra == "all-dev"
 Requires-Dist: pytest-cov (>=2.11.1,<3.0.0) ; extra == "tests" or extra == "all-dev"
 Requires-Dist: pytorch-forecasting (>=0.9.0,<0.10.0) ; extra == "torch" or extra == "all" or extra == "all-dev"
-Requires-Dist: pytorch-lightning ; extra == "torch"
+Requires-Dist: pytorch-lightning ; extra == "torch" or extra == "all" or extra == "all-dev"
 Requires-Dist: pyts (>=0.12.0,<0.13.0) ; extra == "classification" or extra == "all" or extra == "all-dev"
-Requires-Dist: ruptures (==1.1.5)
+Requires-Dist: ruptures (>=1.1.5,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24,<2)
-Requires-Dist: scipy (<1.8.0)
+Requires-Dist: scipy (>=1.0,<2.0)
 Requires-Dist: seaborn (>=0.11.1,<0.12.0)
 Requires-Dist: semver (>=2.13.0,<3.0.0) ; extra == "release" or extra == "all-dev" or extra == "all-dev"
 Requires-Dist: sphinx-mathjax-offline (>=0.0.1,<0.0.2) ; extra == "docs" or extra == "all-dev"
 Requires-Dist: sphinx-rtd-theme (>=0.5.1,<0.6.0) ; extra == "docs" or extra == "all-dev"
+Requires-Dist: sqlalchemy (>=1.1.0,<2.0.0) ; extra == "auto" or extra == "all" or extra == "all-dev"
 Requires-Dist: statsmodels (>=0.12,<0.14)
 Requires-Dist: tbats (>=1.1.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: torch (>=1.8.0,<1.12.0) ; extra == "torch" or extra == "all" or extra == "all-dev"
+Requires-Dist: tsfresh (>=0.20.0,<0.21.0) ; extra == "classification" or extra == "all" or extra == "all-dev"
 Requires-Dist: typer (>=0.4.0,<0.5.0)
 Requires-Dist: types-Deprecated (==1.2.9)
 Requires-Dist: types-PyYAML (>=6.0.0,<7.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: types-setuptools (>=65.7.0,<66.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: typing_extensions
 Requires-Dist: wandb (>=0.12.2,<0.13.0) ; extra == "wandb" or extra == "all" or extra == "all-dev"
 Project-URL: Repository, https://github.com/tinkoff-ai/etna
@@ -238,17 +236,19 @@
 ```bash
 pip install --upgrade pip
 pip install etna
 ```
 
 The default version doesn't contain all the dependencies, because some of them are needed only for specific models, e.g. Prophet, PyTorch.
 Available user extensions are the following:
-* `prophet`
-* `torch`
-* `wandb`
+* `prophet`: adds prophet model`,
+* `torch`: adds models based on neural nets,
+* `wandb`: adds wandb logger,
+* `auto`: adds AutoML functionality,
+* `classiciation`: adds time series classification functionality.
 
 Install extension:
 ```bash
 pip install etna[extension-name]
 ```
 
 Install all extensions:
@@ -288,40 +288,44 @@
 
 ## Documentation
 
 ETNA documentation is available [here](https://etna-docs.netlify.app/).
 
 ## Community
 
-To ask the questions or discuss the library you can join our [telegram chat](t.me/etna_support). 
+To ask the questions or discuss the library you can join our [telegram chat](https://t.me/etna_support). 
 [Discussions section](https://github.com/tinkoff-ai/etna/discussions) on github is also open for this purpose.
 
 ## Resources
 
 - [Forecasting with ETNA: Fast and Furious](https://medium.com/its-tinkoff/forecasting-with-etna-fast-and-furious-1b58e1453809) on Medium
 
 - [ETNA Regressors](https://medium.com/its-tinkoff/etna-regressors-d2722923e88e) on Medium
 
 - [Time series forecasting with ETNA: first steps](https://medium.com/its-tinkoff/time-series-forecasting-with-etna-first-steps-dfaf90c5b919) on Medium
 
 - [ETNA: Time Series Analysis. What, why and how?](https://medium.com/its-tinkoff/etna-time-series-analysis-what-why-and-how-e45557af4f6c) on Medium
 
+- [Time Series Forecasting Strategies in ETNA](https://medium.com/its-tinkoff/time-series-forecasting-strategies-in-etna-93d7d2f8a911) on Medium
+
 - [Tabular Playground Series - Mar 2022 (7th place!)](https://www.kaggle.com/code/chikovalexander/tps-mar-2022-etna/notebook?scriptVersionId=91575908) on Kaggle
 
 - [Store sales prediction with etna library](https://www.kaggle.com/dmitrybunin/store-sales-prediction-with-etna-library?scriptVersionId=81104235) on Kaggle
 
 - [Tabular Playground Series - Jan 2022](https://www.kaggle.com/code/chikovalexander/tps-jan-2022-etna/notebook) on Kaggle
 
 - [EDA notebook for Ubiquant Market Prediction](https://www.kaggle.com/code/martins0n/ubiquant-eda-toy-predictions-etna) on Kaggle
 
 - [PyCon Russia September 2021 talk](https://youtu.be/VxWHLEFgXnE) on YouTube
 
 - [ETNA Meetup Jun 2022](https://www.youtube.com/watch?v=N1Xy3EqY058&list=PLLrf_044z4JrSsjMd-3dF6VbBLPI_yOxG) on YouTube
 
 - [DUMP May 2022 talk](https://youtu.be/12uuxepdtks) on YouTube
+
+- [Прикладные задачи анализа данных, лекция 8 — Временные ряды 2](https://youtu.be/1gXVbidDZck) on YouTube
  
 ## Acknowledgments
 
 ### ETNA.Team
 
 [Andrey Alekseev](https://github.com/iKintosh),
 [Nikita Barinov](https://github.com/diadorer),
@@ -331,15 +335,17 @@
 [Martin Gabdushev](https://github.com/martins0n),
 [Sergey Kolesnikov](https://github.com/Scitator),
 [Artem Makhin](https://github.com/Ama16),
 [Ivan Mitskovets](https://github.com/imitskovets),
 [Albina Munirova](https://github.com/albinamunirova),
 [Julia Shenshina](https://github.com/julia-shenshina),
 [Yuriy Tarasyuk](https://github.com/DBcreator),
-[Konstantin Vedernikov](https://github.com/scanhex12)
+[Konstantin Vedernikov](https://github.com/scanhex12),
+[Ivan Nedosekov](https://github.com/GrozniyToaster),
+[Rodion Petrov](https://github.com/Noidor1)
 
 ### ETNA.Contributors
 
 [WinstonDovlatov](https://github.com/WinstonDovlatov),
 [mvakhmenin](https://github.com/mvakhmenin),
 [Carlosbogo](https://github.com/Carlosbogo),
 [Pacman1984](https://github.com/Pacman1984),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

