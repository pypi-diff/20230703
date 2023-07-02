# Comparing `tmp/lolpop-0.1.0a8.tar.gz` & `tmp/lolpop-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolpop-0.1.0a8.tar", max compression
+gzip compressed data, was "lolpop-0.1.0a9.tar", max compression
```

## Comparing `lolpop-0.1.0a8.tar` & `lolpop-0.1.0a9.tar`

### file list

```diff
@@ -1,167 +1,177 @@
--rw-r--r--   0        0        0    11357 2023-06-15 03:53:18.075554 lolpop-0.1.0a8/LICENSE
--rw-r--r--   0        0        0      373 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/__init__.py
--rw-r--r--   0        0        0     2552 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/cli.py
--rw-r--r--   0        0        0    12841 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/create.py
--rw-r--r--   0        0        0     3464 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/datagen.py
--rw-r--r--   0        0        0      432 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/package.py
--rw-r--r--   0        0        0     1928 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/run.py
--rw-r--r--   0        0        0     2037 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/seed.py
--rw-r--r--   0        0        0      451 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/cli/test.py
--rw-r--r--   0        0        0     1454 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/__init__.py
--rw-r--r--   0        0        0     3752 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/base_component.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/__init__.py
--rw-r--r--   0        0        0      164 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/base_data_checker.py
--rw-r--r--   0        0        0     2356 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/deepchecks_data_checker.py
--rw-r--r--   0        0        0     1813 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/evidentlyai_data_checker.py
--rw-r--r--   0        0        0     2650 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_checker/stumpy_matrix_profiler.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/__init__.py
--rw-r--r--   0        0        0      233 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/base_data_connector.py
--rw-r--r--   0        0        0     6265 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/bigquery_data_connector.py
--rw-r--r--   0        0        0     5431 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/databricks_sql_data_connector.py
--rw-r--r--   0        0        0     4188 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/duckdb_data_connector.py
--rw-r--r--   0        0        0     4275 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/gcs_data_connector.py
--rw-r--r--   0        0        0     1299 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/local_data_connector.py
--rw-r--r--   0        0        0     5453 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/postgres_data_connector.py
--rw-r--r--   0        0        0      637 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/redshift_data_connector.py
--rw-r--r--   0        0        0     3352 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/s3_data_connector.py
--rw-r--r--   0        0        0     6484 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_connector/snowflake_data_connector.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/__init__.py
--rw-r--r--   0        0        0      243 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/base_data_profiler.py
--rw-r--r--   0        0        0     1462 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/continual_data_profiler.py
--rw-r--r--   0        0        0     2314 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/evidentlyai_data_profiler.py
--rw-r--r--   0        0        0     2162 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/sweetviz_data_profiler.py
--rw-r--r--   0        0        0     1087 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/tslumen_data_profiler.py
--rw-r--r--   0        0        0     2164 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_splitter/__init__.py
--rw-r--r--   0        0        0      163 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_splitter/base_data_splitter.py
--rw-r--r--   0        0        0     9807 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_splitter/local_data_splitter.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_synthesizer/__init__.py
--rw-r--r--   0        0        0      396 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_synthesizer/base_data_synthesizer.py
--rw-r--r--   0        0        0     5878 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_synthesizer/svd_data_synthesizer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/__init__.py
--rw-r--r--   0        0        0      301 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/base_data_transformer.py
--rw-r--r--   0        0        0      712 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/bigquery_data_transformer.py
--rw-r--r--   0        0        0      870 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/databricks_sql_data_transformer.py
--rw-r--r--   0        0        0     4525 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/dbt_data_transformer.py
--rw-r--r--   0        0        0      613 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/duckdb_data_transformer.py
--rw-r--r--   0        0        0     2484 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/local_data_transformer.py
--rw-r--r--   0        0        0      838 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/postrgres_data_transformer.py
--rw-r--r--   0        0        0      962 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/redshift_data_transformer.py
--rw-r--r--   0        0        0      855 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/data_transformer/snowflake_data_transformer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/genai_chatbot/__init__.py
--rw-r--r--   0        0        0      228 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/genai_chatbot/base_genai_chatbot.py
--rw-r--r--   0        0        0      940 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/genai_chatbot/openai_chatbot.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/__init__.py
--rw-r--r--   0        0        0     2705 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
--rw-r--r--   0        0        0     2755 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
--rw-r--r--   0        0        0     9416 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/__init__.py
--rw-r--r--   0        0        0      139 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/base_logger.py
--rw-r--r--   0        0        0     1699 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/file_logger.py
--rw-r--r--   0        0        0     2017 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/logger/stdout_logger.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.079554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/__init__.py
--rw-r--r--   0        0        0     2073 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/base_metadata_tracker.py
--rw-r--r--   0        0        0    15598 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/continual_metadata_tracker.py
--rw-r--r--   0        0        0    12571 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/__init__.py
--rw-r--r--   0        0        0      460 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/base_metrics_tracker.py
--rw-r--r--   0        0        0     5843 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/continual_metrics_tracker.py
--rw-r--r--   0        0        0     4804 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_bias_checker/__init__.py
--rw-r--r--   0        0        0     4876 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
--rw-r--r--   0        0        0      240 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_bias_checker/base_model_bias_checker.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/__init__.py
--rw-r--r--   0        0        0    11210 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/base_model_checker.py
--rw-r--r--   0        0        0     2846 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/deepchecks_model_checker.py
--rw-r--r--   0        0        0     3601 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_checker/evidentlyai_model_checker.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_deployer/__init__.py
--rw-r--r--   0        0        0      371 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_deployer/base_model_deployer.py
--rw-r--r--   0        0        0      574 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_deployer/seldon_model_deployer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_explainer/__init__.py
--rw-r--r--   0        0        0    10342 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_explainer/alibi_model_explainer.py
--rw-r--r--   0        0        0      244 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_explainer/base_model_explainer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/__init__.py
--rw-r--r--   0        0        0      309 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/base_model_repository.py
--rw-r--r--   0        0        0     2993 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/continual_model_repository.py
--rw-r--r--   0        0        0     4521 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_repository/mlflow_model_repository.py
--rw-r--r--   0        0        0     5064 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/ProphetModelTrainer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/__init__.py
--rw-r--r--   0        0        0    12320 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/base_model_trainer.py
--rw-r--r--   0        0        0     2404 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_trainer/xgboost_model_trainer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/__init__.py
--rw-r--r--   0        0        0      169 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/base_model_visualizer.py
--rw-r--r--   0        0        0     2504 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/prophet_visualizer.py
--rw-r--r--   0        0        0     5102 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/__init__.py
--rw-r--r--   0        0        0      156 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/base_notifier.py
--rw-r--r--   0        0        0     2904 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/gmail_notifier.py
--rw-r--r--   0        0        0      880 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/slack_notifier.py
--rw-r--r--   0        0        0     1272 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/smtp_notifier.py
--rw-r--r--   0        0        0      322 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/notifier/stdout_notifier.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/__init__.py
--rw-r--r--   0        0        0      376 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/base_resource_version_control.py
--rw-r--r--   0        0        0     3221 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/continual_version_control.py
--rw-r--r--   0        0        0     5828 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/component/resource_version_control/dvc_version_control.py
--rw-r--r--   0        0        0     2802 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/extension/__init__.py
--rw-r--r--   0        0        0     1376 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/__init__.py
--rw-r--r--   0        0        0     4971 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/base_pipeline.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/__init__.py
--rw-r--r--   0        0        0      454 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/base_deploy.py
--rw-r--r--   0        0        0     3849 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/metaflow_offline_deploy.py
--rw-r--r--   0        0        0     1660 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/deploy/offline_deploy.py
--rw-r--r--   0        0        0       42 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/__init__.py
--rw-r--r--   0        0        0      227 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/base_predict.py
--rw-r--r--   0        0        0     7180 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/metaflow_offline_predict.py
--rw-r--r--   0        0        0     4172 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/predict/offline_predict.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/__init__.py
--rw-r--r--   0        0        0      452 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/base_process.py
--rw-r--r--   0        0        0     5660 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/metaflow_offline_process.py
--rw-r--r--   0        0        0     3267 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/process/offline_process.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/__init__.py
--rw-r--r--   0        0        0      645 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/base_train.py
--rw-r--r--   0        0        0     7331 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/metaflow_offline_train.py
--rw-r--r--   0        0        0     4499 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/train/offline_train.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0      275 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/wrapper/base_wrapper.py
--rw-r--r--   0        0        0      793 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
--rw-r--r--   0        0        0     1361 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/__init__.py
--rw-r--r--   0        0        0     7059 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/base_runner.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/classification_runner/__init__.py
--rw-r--r--   0        0        0     7732 2023-06-15 03:53:18.083554 lolpop-0.1.0a8/lolpop/runner/classification_runner/classification_runner.py
--rw-r--r--   0        0        0     6194 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/classification_runner/metaflow_classification.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/regression_runner/__init__.py
--rw-r--r--   0        0        0      397 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/regression_runner/regression_runner.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/timeseries_runner/__init__.py
--rw-r--r--   0        0        0     8862 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/runner/timeseries_runner/timeseries_runner.py
--rw-r--r--   0        0        0      175 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
--rw-r--r--   0        0        0      802 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
--rw-r--r--   0        0        0     1122 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
--rw-r--r--   0        0        0      167 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
--rw-r--r--   0        0        0      803 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
--rw-r--r--   0        0        0     1096 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
--rw-r--r--   0        0        0       66 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0       32 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
--rw-r--r--   0        0        0      152 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/__int__.py
--rw-r--r--   0        0        0      152 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
--rw-r--r--   0        0        0      310 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      151 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
--rw-r--r--   0        0        0      795 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
--rw-r--r--   0        0        0     1054 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
--rw-r--r--   0        0        0        0 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/__init__.py
--rw-r--r--   0        0        0    15773 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/common_utils.py
--rw-r--r--   0        0        0     1566 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/continual_utils.py
--rw-r--r--   0        0        0     2452 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/metaflow_utils.py
--rw-r--r--   0        0        0     3298 2023-06-15 03:53:18.087555 lolpop-0.1.0a8/lolpop/utils/mlflow_utils.py
--rw-r--r--   0        0        0     2433 2023-06-15 03:53:33.856530 lolpop-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 lolpop-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-02 22:42:36.930884 lolpop-0.1.0a9/LICENSE
+-rw-r--r--   0        0        0      373 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0     2595 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/cli.py
+-rw-r--r--   0        0        0    14065 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/create.py
+-rw-r--r--   0        0        0     3464 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/datagen.py
+-rw-r--r--   0        0        0      931 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/extension.py
+-rw-r--r--   0        0        0     1209 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/extensions/__init__.py
+-rw-r--r--   0        0        0      432 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/package.py
+-rw-r--r--   0        0        0     1928 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/run.py
+-rw-r--r--   0        0        0     2037 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/seed.py
+-rw-r--r--   0        0        0     3265 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/cli/test.py
+-rw-r--r--   0        0        0     1454 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/__init__.py
+-rw-r--r--   0        0        0     4204 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/base_component.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_checker/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_checker/base_data_checker.py
+-rw-r--r--   0        0        0     2356 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_checker/deepchecks_data_checker.py
+-rw-r--r--   0        0        0     1813 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_checker/evidentlyai_data_checker.py
+-rw-r--r--   0        0        0     2621 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_checker/stumpy_matrix_profiler.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/base_data_connector.py
+-rw-r--r--   0        0        0     6265 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/bigquery_data_connector.py
+-rw-r--r--   0        0        0     5431 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/databricks_sql_data_connector.py
+-rw-r--r--   0        0        0     4188 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/duckdb_data_connector.py
+-rw-r--r--   0        0        0     4275 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/gcs_data_connector.py
+-rw-r--r--   0        0        0     1299 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/local_data_connector.py
+-rw-r--r--   0        0        0     5453 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/postgres_data_connector.py
+-rw-r--r--   0        0        0      637 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/redshift_data_connector.py
+-rw-r--r--   0        0        0     3352 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/s3_data_connector.py
+-rw-r--r--   0        0        0     6484 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_connector/snowflake_data_connector.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/__init__.py
+-rw-r--r--   0        0        0      243 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/base_data_profiler.py
+-rw-r--r--   0        0        0     1462 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/continual_data_profiler.py
+-rw-r--r--   0        0        0     2314 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/evidentlyai_data_profiler.py
+-rw-r--r--   0        0        0     2162 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/sweetviz_data_profiler.py
+-rw-r--r--   0        0        0     1087 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/tslumen_data_profiler.py
+-rw-r--r--   0        0        0     2164 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_splitter/__init__.py
+-rw-r--r--   0        0        0      163 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_splitter/base_data_splitter.py
+-rw-r--r--   0        0        0     9807 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_splitter/local_data_splitter.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_synthesizer/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_synthesizer/base_data_synthesizer.py
+-rw-r--r--   0        0        0     5878 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_synthesizer/svd_data_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/base_data_transformer.py
+-rw-r--r--   0        0        0      712 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/bigquery_data_transformer.py
+-rw-r--r--   0        0        0      870 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/databricks_sql_data_transformer.py
+-rw-r--r--   0        0        0     4525 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/dbt_data_transformer.py
+-rw-r--r--   0        0        0      613 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/duckdb_data_transformer.py
+-rw-r--r--   0        0        0     2484 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/local_data_transformer.py
+-rw-r--r--   0        0        0      838 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/postrgres_data_transformer.py
+-rw-r--r--   0        0        0      962 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/redshift_data_transformer.py
+-rw-r--r--   0        0        0      855 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/data_transformer/snowflake_data_transformer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/genai_chatbot/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/genai_chatbot/base_genai_chatbot.py
+-rw-r--r--   0        0        0      940 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/genai_chatbot/openai_chatbot.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/__init__.py
+-rw-r--r--   0        0        0     2705 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     2755 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     9416 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/logger/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/logger/base_logger.py
+-rw-r--r--   0        0        0     2342 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/logger/file_logger.py
+-rw-r--r--   0        0        0     2082 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/logger/stdout_logger.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metadata_tracker/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metadata_tracker/base_metadata_tracker.py
+-rw-r--r--   0        0        0    15598 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metadata_tracker/continual_metadata_tracker.py
+-rw-r--r--   0        0        0    12571 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metrics_tracker/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metrics_tracker/base_metrics_tracker.py
+-rw-r--r--   0        0        0     5843 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metrics_tracker/continual_metrics_tracker.py
+-rw-r--r--   0        0        0     4804 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_bias_checker/__init__.py
+-rw-r--r--   0        0        0     4876 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
+-rw-r--r--   0        0        0      240 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_bias_checker/base_model_bias_checker.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_checker/__init__.py
+-rw-r--r--   0        0        0    11210 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_checker/base_model_checker.py
+-rw-r--r--   0        0        0     2846 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_checker/deepchecks_model_checker.py
+-rw-r--r--   0        0        0     3601 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_checker/evidentlyai_model_checker.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_deployer/__init__.py
+-rw-r--r--   0        0        0      371 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_deployer/base_model_deployer.py
+-rw-r--r--   0        0        0      574 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_deployer/seldon_model_deployer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_explainer/__init__.py
+-rw-r--r--   0        0        0    10342 2023-07-02 22:42:36.934885 lolpop-0.1.0a9/lolpop/component/model_explainer/alibi_model_explainer.py
+-rw-r--r--   0        0        0      244 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_explainer/base_model_explainer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_repository/__init__.py
+-rw-r--r--   0        0        0      309 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_repository/base_model_repository.py
+-rw-r--r--   0        0        0     2993 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_repository/continual_model_repository.py
+-rw-r--r--   0        0        0     4521 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_repository/mlflow_model_repository.py
+-rw-r--r--   0        0        0     5064 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_trainer/ProphetModelTrainer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_trainer/__init__.py
+-rw-r--r--   0        0        0    12320 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_trainer/base_model_trainer.py
+-rw-r--r--   0        0        0     2404 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_trainer/xgboost_model_trainer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_visualizer/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_visualizer/base_model_visualizer.py
+-rw-r--r--   0        0        0     2504 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_visualizer/prophet_visualizer.py
+-rw-r--r--   0        0        0     5102 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/notifier/__init__.py
+-rw-r--r--   0        0        0      156 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/notifier/base_notifier.py
+-rw-r--r--   0        0        0     2904 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/notifier/gmail_notifier.py
+-rw-r--r--   0        0        0      880 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/notifier/slack_notifier.py
+-rw-r--r--   0        0        0     1272 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/notifier/smtp_notifier.py
+-rw-r--r--   0        0        0      322 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/notifier/stdout_notifier.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/resource_version_control/__init__.py
+-rw-r--r--   0        0        0      376 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/resource_version_control/base_resource_version_control.py
+-rw-r--r--   0        0        0     3221 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/resource_version_control/continual_version_control.py
+-rw-r--r--   0        0        0     5828 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/resource_version_control/dvc_version_control.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/test_recorder/__init__.py
+-rw-r--r--   0        0        0      293 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/test_recorder/base_test_recorder.py
+-rw-r--r--   0        0        0      929 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/component/test_recorder/local_test_recorder.py
+-rw-r--r--   0        0        0     2802 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0     1376 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/__init__.py
+-rw-r--r--   0        0        0     5547 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/deploy/__init__.py
+-rw-r--r--   0        0        0      454 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/deploy/base_deploy.py
+-rw-r--r--   0        0        0     3849 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/deploy/metaflow_offline_deploy.py
+-rw-r--r--   0        0        0     1660 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/deploy/offline_deploy.py
+-rw-r--r--   0        0        0       42 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/predict/__init__.py
+-rw-r--r--   0        0        0      227 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/predict/base_predict.py
+-rw-r--r--   0        0        0     7180 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/predict/metaflow_offline_predict.py
+-rw-r--r--   0        0        0     4172 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/predict/offline_predict.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/process/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/process/base_process.py
+-rw-r--r--   0        0        0     5660 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/process/metaflow_offline_process.py
+-rw-r--r--   0        0        0     3267 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/process/offline_process.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/train/__init__.py
+-rw-r--r--   0        0        0      645 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/train/base_train.py
+-rw-r--r--   0        0        0     7331 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/train/metaflow_offline_train.py
+-rw-r--r--   0        0        0     4499 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/train/offline_train.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/wrapper/base_wrapper.py
+-rw-r--r--   0        0        0      793 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
+-rw-r--r--   0        0        0     1361 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/__init__.py
+-rw-r--r--   0        0        0     5794 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/base_runner.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/classification_runner/__init__.py
+-rw-r--r--   0        0        0     7732 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/classification_runner/classification_runner.py
+-rw-r--r--   0        0        0     6194 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/classification_runner/metaflow_classification.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/regression_runner/__init__.py
+-rw-r--r--   0        0        0      397 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/regression_runner/regression_runner.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/timeseries_runner/__init__.py
+-rw-r--r--   0        0        0     8862 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/runner/timeseries_runner/timeseries_runner.py
+-rw-r--r--   0        0        0      112 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/cli_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/cli_template/{{cookiecutter.cli_command}}/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/cli_template/{{cookiecutter.cli_command}}/{{cookiecutter.cli_command}}.py
+-rw-r--r--   0        0        0      175 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/component_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
+-rw-r--r--   0        0        0      802 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
+-rw-r--r--   0        0        0     1122 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
+-rw-r--r--   0        0        0      167 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/pipeline_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
+-rw-r--r--   0        0        0      803 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
+-rw-r--r--   0        0        0     1096 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
+-rw-r--r--   0        0        0       66 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0       32 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
+-rw-r--r--   0        0        0      152 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/__int__.py
+-rw-r--r--   0        0        0      152 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/cli/extensions/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
+-rw-r--r--   0        0        0      310 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/runner_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
+-rw-r--r--   0        0        0      795 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
+-rw-r--r--   0        0        0     1054 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
+-rw-r--r--   0        0        0        0 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/utils/__init__.py
+-rw-r--r--   0        0        0    26000 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/utils/common_utils.py
+-rw-r--r--   0        0        0     1566 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/utils/continual_utils.py
+-rw-r--r--   0        0        0     2452 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/utils/metaflow_utils.py
+-rw-r--r--   0        0        0     3298 2023-07-02 22:42:36.938885 lolpop-0.1.0a9/lolpop/utils/mlflow_utils.py
+-rw-r--r--   0        0        0     2433 2023-07-02 22:42:51.914921 lolpop-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0     2914 1970-01-01 00:00:00.000000 lolpop-0.1.0a9/PKG-INFO
```

### Comparing `lolpop-0.1.0a8/LICENSE` & `lolpop-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/cli/cli.py` & `lolpop-0.1.0a9/lolpop/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import typer 
-import click 
 import os 
 
-from lolpop.cli import create, run, package, test, datagen, seed 
+from lolpop.cli import create, run, package, test, datagen, seed, extension
 from importlib.metadata import version
 from typing import Optional
 from pathlib import Path 
 from cookiecutter.main import cookiecutter
 from lolpop import __template_path__ as lolpop_template_path
 from typer.core import TyperGroup 
 
@@ -25,14 +24,15 @@
 
 app.add_typer(run.app, name="run")
 app.add_typer(create.app, name="create")
 app.add_typer(datagen.app, name="datagen")
 app.add_typer(seed.app, name="seed")
 app.add_typer(test.app, name="test")
 app.add_typer(package.app, name="package")
+app.add_typer(extension.app, name="extension")
 
 
 
 def version_callback(value: bool):
     if value:
         try:
             typer.secho("lolpop version: %s" % __version__, fg="blue")
```

### Comparing `lolpop-0.1.0a8/lolpop/cli/create.py` & `lolpop-0.1.0a9/lolpop/cli/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,50 +30,77 @@
         typer.echo(ctx.command.get_help(ctx))
 
 
 @app.command("component", help="Initialize a custom component.")
 def component(
     component_type: str = typer.Argument(..., help="Component type (Should be snake_case)."),
     component_class: str = typer.Argument(..., help="Component class name (Should be snake_case)."),
-    extension_name: str = typer.Argument(None, help = "Name of the parent extension for this resource."),
-    template_path: str = typer.Argument(
+    extension_name: str = typer.Argument(..., help = "Name of the parent extension for this resource."),
+    template_path: str = typer.Option(
         lolpop_template_path + "/component_template", help="Path to the template file. Or a git url of a template file."),
     project_dir: Path = typer.Option(os.getcwd(), help="Project directory for the new component."),
 ): 
     create_template("component", component_type,
                     component_class, template_path, project_dir, extension_name)
     
 
 @app.command("pipeline", help="Initialize a custom pipeline.")
 def pipeline(
     pipeline_type: str = typer.Argument(..., help="Pipeline type (Should be snake_case)."),
     pipeline_class: str = typer.Argument(
         ..., help="Pipeline class name (Should be snake_case)."),
     extension_name: str = typer.Argument(
-            None, help="Name of the parent extension for this resource."),
-    template_path: str = typer.Argument(
+            ..., help="Name of the parent extension for this resource."),
+    template_path: str = typer.Option(
         lolpop_template_path + "/pipeline_template", help="Path to the template file. Or a git url of a template file."),
     project_dir: Path = typer.Option(os.getcwd(), help="Parent directory for the new pipeline."),
 ): 
     create_template("pipeline", pipeline_type,
                     pipeline_class, template_path, project_dir, extension_name)
 
 
 @app.command("runner", help="Initialize a custom component.")
 def runner(
     runner_type: str = typer.Argument(..., help="Component type (Should be snake_case)"),
     runner_class: str = typer.Argument(..., help="Component class name (Should be snake_case)."),
-    extension_name: str = typer.Argument(None, help="Name of the parent extension for this resource."),
-    template_path: str = typer.Argument(
+    extension_name: str = typer.Argument(..., help="Name of the parent extension for this resource."),
+    template_path: str = typer.Option(
         lolpop_template_path + "/runner_template", help="Path to the template file. Or a git url of a template file."),
     project_dir: Path = typer.Option(os.getcwd(), help="Parent directory for the new component."),
 ): 
     create_template("runner", runner_type,
                     runner_class, template_path, project_dir, extension_name)
     
+
+@app.command("cli-command", help="Initialize a custom component.")
+def cli_command(
+    command_name: str = typer.Argument(
+        ..., help="Name of the cli command to create."),
+    template_path: str = typer.Option(
+        lolpop_template_path + "/cli_template", help="Path to the template file. Or a git url of a template file."),
+    command_description: str = typer.Option(None, help="description for the command_name"),
+    project_dir: Path = typer.Option(
+        os.getcwd(), help="Parent directory for the new component."),
+):
+    typer.secho("Creating template for %s" %command_name, fg="blue")
+    try:
+        output_dir = "%s/lolpop/cli/extensions/" % (project_dir)
+        cookiecutter(template=template_path,
+                     extra_context={
+                         "cli_command": command_name,
+                         "command_description": command_description,
+                     },
+                     output_dir=output_dir, no_input=True)
+        typer.secho("Successfully created template at location %s" %
+                    output_dir, fg="green")
+    except Exception as e:
+        typer.secho("Failed to create template for %s: %s" %
+                    (command_name, str(e)), fg="red")
+
+    
 #template type = component, pipeline, runner, 
 def create_template(template_type, object_type, object_class, template_path, project_dir, extension_name): 
     typer.secho("Creating template for %s %s" %(template_type, object_class), fg="blue")
     try: 
         object_class_camel = ''.join([i.title() for i in object_class.split("_")])
         object_type_camel = ''.join([i.title() for i in object_type.split("_")])
         #TODO: Check if object_type already exists and just copy a new template in that
```

### Comparing `lolpop-0.1.0a8/lolpop/cli/datagen.py` & `lolpop-0.1.0a9/lolpop/cli/datagen.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/cli/run.py` & `lolpop-0.1.0a9/lolpop/cli/run.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/cli/seed.py` & `lolpop-0.1.0a9/lolpop/cli/seed.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/__init__.py` & `lolpop-0.1.0a9/lolpop/component/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/base_component.py` & `lolpop-0.1.0a9/lolpop/component/base_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from lolpop.utils import common_utils as utils
 from omegaconf import OmegaConf
 from inspect import currentframe
+
 class BaseComponent: 
     __REQUIRED_CONF__ = {
         "config" : []
     }
     __DEFAULT_CONF__ = {
         "config" : {}
     }
@@ -12,14 +13,16 @@
     suppress_logger = False
     suppress_notifier = False 
 
     def __init__(self, conf={}, pipeline_conf={}, runner_conf={}, parent_process=None, problem_type = None, 
                  components = {}, skip_config_validation=False, *args, **kwargs):
         #set basic properties, like name and configs
         self.name = type(self).__name__
+        self.type = self.__module__.split(".")[-2]
+        self.integration_type = self.__module__.split(".")[-1]
         config = utils.get_conf(conf)
         self.pipeline_conf = pipeline_conf
         self.runner_conf = runner_conf
         self.parent_process = parent_process
         self.problem_type = problem_type
 
         #resolve variables
@@ -37,14 +40,19 @@
                         )
 
         #Now we validate config to make sure the component has everything it needs
         if not skip_config_validation: 
             self._validate_conf(valid_conf, components)
         self.config = omega_conf.get("config", {})
 
+        #handle default components: logger, notifier, metadata_tracker
+        components = utils.set_up_default_components(self, valid_conf, self.runner_conf,
+                                                     skip_config_validation=skip_config_validation,
+                                                     components=components)
+
         #if the config looks good, then we can set all our components 
         for component in components.keys(): 
             setattr(self, component, components.get(component))
         
     def _update_components(self, components = {}, *args, **kwargs): 
         for component in components.keys(): 
             setattr(self, component, components.get(component))
```

### Comparing `lolpop-0.1.0a8/lolpop/component/data_checker/deepchecks_data_checker.py` & `lolpop-0.1.0a9/lolpop/component/data_checker/deepchecks_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_checker/evidentlyai_data_checker.py` & `lolpop-0.1.0a9/lolpop/component/data_checker/evidentlyai_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_checker/stumpy_matrix_profiler.py` & `lolpop-0.1.0a9/lolpop/component/data_checker/stumpy_matrix_profiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
         file_path = "%s/STUMP_DISCORD_ANALSIS.PNG" % self._get_config("local_dir")
         plt.savefig(file_path)
 
         return None, file_path, "PASS"
 
     def _plot_mp(self, axs, m, h, mp, discords, i): 
-        print("i:" + str(i))
         axs[i].set_ylabel('MP (m=%s)' %m, fontsize='10')
         axs[i].set_xlabel('Time', fontsize='10')
         axs[i].plot(mp[:, 0])
          
         for discord_idx in discords: 
             if i == 1:  # only add rectangles for the first window, otherwise it's going to get cluttered.
                 rect = Rectangle((discord_idx, 0), m, h, facecolor='lightgrey')
```

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/bigquery_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/bigquery_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/databricks_sql_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/databricks_sql_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/duckdb_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/duckdb_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/gcs_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/gcs_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/local_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/local_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/postgres_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/postgres_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/redshift_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/redshift_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/s3_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/s3_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_connector/snowflake_data_connector.py` & `lolpop-0.1.0a9/lolpop/component/data_connector/snowflake_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_profiler/continual_data_profiler.py` & `lolpop-0.1.0a9/lolpop/component/data_profiler/continual_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_profiler/evidentlyai_data_profiler.py` & `lolpop-0.1.0a9/lolpop/component/data_profiler/evidentlyai_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_profiler/sweetviz_data_profiler.py` & `lolpop-0.1.0a9/lolpop/component/data_profiler/sweetviz_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_profiler/tslumen_data_profiler.py` & `lolpop-0.1.0a9/lolpop/component/data_profiler/tslumen_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_profiler/ydata_profiling_data_profiler.py` & `lolpop-0.1.0a9/lolpop/component/data_profiler/ydata_profiling_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_splitter/local_data_splitter.py` & `lolpop-0.1.0a9/lolpop/component/data_splitter/local_data_splitter.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_synthesizer/svd_data_synthesizer.py` & `lolpop-0.1.0a9/lolpop/component/data_synthesizer/svd_data_synthesizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/bigquery_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/bigquery_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/databricks_sql_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/databricks_sql_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/dbt_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/dbt_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/duckdb_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/duckdb_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/local_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/local_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/postrgres_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/postrgres_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/redshift_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/redshift_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/data_transformer/snowflake_data_transformer.py` & `lolpop-0.1.0a9/lolpop/component/data_transformer/snowflake_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/genai_chatbot/openai_chatbot.py` & `lolpop-0.1.0a9/lolpop/component/genai_chatbot/openai_chatbot.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py` & `lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py` & `lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py` & `lolpop-0.1.0a9/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/logger/file_logger.py` & `lolpop-0.1.0a9/lolpop/component/logger/file_logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,44 +2,58 @@
 import logging 
 from datetime import datetime 
 class FileLogger(BaseLogger): 
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         filename = self._get_config("log_filename","lolpop.log")
+        self.url = filename 
         level = self._get_config("log_level", "INFO")
-        logging.basicConfig(filename=filename, level=level) 
+        if isinstance(level, str):
+            level = self._get_level_value(level)
+        format = self._get_config("log_format", "%(message)s")
 
-    def log(self, msg, level, time = None, process_name=None, line_num=None, *args, **kwargs): 
-        if self._get_level_value(level) <= self._get_level_value(self._get_config("log_level", "DEBUG")):
+        logger = logging.getLogger("lolpop")
+        logger.setLevel(level)
+        file_handler = logging.FileHandler(filename)
+        file_handler.setLevel(level)
+        file_handler.setFormatter(logging.Formatter(format))
+        logger.addHandler(file_handler)
+
+        self.logger = logger
+        logger.log(30, "\n\n")
+        self.log("Initialized logger for lolpop workflow.", level="INFO")
+
+    def log(self, msg, level="INFO", time = None, process_name=None, line_num=None, *args, **kwargs): 
+        if self._get_level_value(level) >= self._get_level_value(self._get_config("log_level", "DEBUG")):
             msg_out = ""
             if not time:
                 time = datetime.utcnow().strftime("%Y/%m/%d %H:%M:%S.%f")
             msg_out = msg_out + "%s [%s] " % (time, level)
             if process_name:
                 msg_out = msg_out + \
                     "<%s" % (process_name)
                 if line_num and self._get_config("use_line_numbers", False):
                     msg_out = msg_out + \
                         "|%s> ::: %s" % (
                             line_num, msg)
                 else:
                     msg_out = msg_out + "> ::: %s" % msg
-            logging.log(level, msg, **kwargs)
+            else: 
+                msg_out = msg_out + "::: %s" % msg
+            self.logger.log(self._get_level_value(level), msg_out, **kwargs)
 
     def _get_level_value(self, level):
-        if level == "NONE":
-            return 0
-        elif level == "FATAL":
-            return 1
+        if level == "FATAL" or level == "CRITICAL":
+            return 50
         elif level == "ERROR":
-            return 2
+            return 40
         elif level == "WARN" or level == "WARNING":
-            return 3
+            return 30
         elif level == "INFO":
-            return 4
-        elif level == "DEBUG":
-            return 5
-        elif level == "TRACE":
-            return 6
+            return 20
+        elif level == "DEBUG" or level == "TRACE":
+            return 10
         elif level == "ALL":
-            return 100
+            return 1
+        else: #level == "NONE" or level == "NOTSET":
+            return 0
```

### Comparing `lolpop-0.1.0a8/lolpop/component/logger/stdout_logger.py` & `lolpop-0.1.0a9/lolpop/component/logger/stdout_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
             if process_name: 
                 msg_out = msg_out + "<%s%s%s" %(Fore.BLUE,process_name,Style.RESET_ALL)
                 if line_num and self._get_config("use_line_numbers",False): 
                     msg_out = msg_out + \
                         "|%s%s%s> ::: %s" % (Fore.GREEN, line_num, Style.RESET_ALL,  msg)
                 else: 
                     msg_out = msg_out + "> ::: %s" %msg
+            else: 
+                msg_out = msg_out + "::: msg"
             print(msg_out)
 
     def _get_level_value(self, level): 
         if level == "NONE": 
             return 0 
         elif level == "FATAL":
             return 1
```

### Comparing `lolpop-0.1.0a8/lolpop/component/metadata_tracker/base_metadata_tracker.py` & `lolpop-0.1.0a9/lolpop/component/metadata_tracker/base_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/metadata_tracker/continual_metadata_tracker.py` & `lolpop-0.1.0a9/lolpop/component/metadata_tracker/continual_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py` & `lolpop-0.1.0a9/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/metrics_tracker/continual_metrics_tracker.py` & `lolpop-0.1.0a9/lolpop/component/metrics_tracker/continual_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py` & `lolpop-0.1.0a9/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py` & `lolpop-0.1.0a9/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_checker/base_model_checker.py` & `lolpop-0.1.0a9/lolpop/component/model_checker/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_checker/deepchecks_model_checker.py` & `lolpop-0.1.0a9/lolpop/component/model_checker/deepchecks_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_checker/evidentlyai_model_checker.py` & `lolpop-0.1.0a9/lolpop/component/model_checker/evidentlyai_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_deployer/seldon_model_deployer.py` & `lolpop-0.1.0a9/lolpop/component/model_deployer/seldon_model_deployer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_explainer/alibi_model_explainer.py` & `lolpop-0.1.0a9/lolpop/component/model_explainer/alibi_model_explainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_repository/continual_model_repository.py` & `lolpop-0.1.0a9/lolpop/component/model_repository/continual_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_repository/mlflow_model_repository.py` & `lolpop-0.1.0a9/lolpop/component/model_repository/mlflow_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_trainer/ProphetModelTrainer.py` & `lolpop-0.1.0a9/lolpop/component/model_trainer/ProphetModelTrainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_trainer/base_model_trainer.py` & `lolpop-0.1.0a9/lolpop/component/model_trainer/base_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_trainer/xgboost_model_trainer.py` & `lolpop-0.1.0a9/lolpop/component/model_trainer/xgboost_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_visualizer/prophet_visualizer.py` & `lolpop-0.1.0a9/lolpop/component/model_visualizer/prophet_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py` & `lolpop-0.1.0a9/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/notifier/gmail_notifier.py` & `lolpop-0.1.0a9/lolpop/component/notifier/gmail_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/notifier/slack_notifier.py` & `lolpop-0.1.0a9/lolpop/component/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/notifier/smtp_notifier.py` & `lolpop-0.1.0a9/lolpop/component/notifier/smtp_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/resource_version_control/continual_version_control.py` & `lolpop-0.1.0a9/lolpop/component/resource_version_control/continual_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/component/resource_version_control/dvc_version_control.py` & `lolpop-0.1.0a9/lolpop/component/resource_version_control/dvc_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/extension/__init__.py` & `lolpop-0.1.0a9/lolpop/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/__init__.py` & `lolpop-0.1.0a9/lolpop/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/base_pipeline.py` & `lolpop-0.1.0a9/lolpop/pipeline/base_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,31 +15,39 @@
     suppress_notifier = False
 
     def __init__(self, conf={}, runner_conf={}, parent_process="runner", problem_type=None, 
                  pipeline_type="base_pipeline", components={}, plugin_mods=[], plugin_paths=[], 
                  skip_config_validation=False, *args, **kwargs):
         #set basic properties like configs
         self.name = type(self).__name__
+        self.type = self.__module__.split(".")[-2]
+        self.integration_type = self.__module__.split(".")[-1]
         conf = utils.get_conf(conf)
         self.parent_process = parent_process
         self.pipeline_type = pipeline_type
         self.runner_conf = runner_conf
         self.problem_type = problem_type
 
         #resolve any variables
         conf = utils.resolve_conf_variables(conf)
         #merge into default conf
-        omega_conf = utils.copy_config_into(OmegaConf.create(conf), self.__DEFAULT_CONF__)
+        conf = utils.copy_config_into(OmegaConf.create(conf), self.__DEFAULT_CONF__)
         #merge pipeline conf into runner conf
-        valid_conf = omega_conf.copy()
+        valid_conf = conf.copy()
         OmegaConf.update(valid_conf, "config", utils.copy_config_into(valid_conf.get("config", {}), runner_conf))
         #validate configuration
         if not skip_config_validation:
-            self._validate_conf(valid_conf, components)
-        self.config = omega_conf.get("config", {})
+            valid_conf = self._validate_conf(valid_conf, components)
+        self.config = conf.get("config", {})
+
+        #handle default components: logger, notifier, metadata_tracker
+        components = utils.set_up_default_components(self, valid_conf, self.runner_conf,
+                                                            plugin_mods=plugin_mods,
+                                                            skip_config_validation=skip_config_validation,
+                                                            components=components)
 
         #set up reference to each component that is passed in from runner. 
         for component in components.keys(): 
             setattr(self, component, components.get(component))
 
         pipeline_conf = self.config
         pipeline_conf["pipeline_type"]=self.pipeline_type
@@ -54,15 +62,15 @@
             plugin_mods = utils.get_plugin_mods(self, plugin_paths, file_path)
         self.plugin_mods = plugin_mods
 
         #now handle all components explicitly set for pipeline
         #note: this will override any component name inherited from the runner, which is what we want
         pipeline_components = {}
         if "components" in conf.keys(): 
-            for component in conf.components.keys(): 
+            for component in conf.get("components",{}).keys(): 
                 obj = utils.register_component_class(self, conf, component, pipeline_conf = pipeline_conf, 
                                                      runner_conf = runner_conf, parent_process=self.name, 
                                                      problem_type = self.problem_type, dependent_components=components, 
                                                      plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
                 if obj is not None: 
                     self.log("Loaded class %s into component %s" %(type(getattr(self, component)).__name__, component))
                     pipeline_components[component] = obj
@@ -80,14 +88,15 @@
             #check to see if missing components are provided by runner via kwargs
             if len(missing.get("components")) > 0: 
                 for component in missing.get("components"): 
                     if components.get(component, None) is not None: 
                         total_missing = total_missing - 1
             if total_missing > 0:   
                 raise Exception ("Missing the following from pipeline configuration: %s" %missing)
+        return conf
 
     def log(self, msg, level="INFO", **kwargs): 
         if not self.suppress_logger: 
             self.logger.log(msg, level, process_name=self.name,
                             line_num=currentframe().f_back.f_lineno, **kwargs)
 
     def notify(self, msg, level="ERROR"): 
@@ -101,8 +110,8 @@
         value = utils.lower_conf(self.config).get(key, None)
         if value is None: 
             value = utils.lower_conf(self.runner_conf).get(key, default_value)
         return value 
 
     def _set_config(self, key, value): 
         key = key.lower()
-        self.config[key]=value
+        self.config[key]=value
```

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/deploy/metaflow_offline_deploy.py` & `lolpop-0.1.0a9/lolpop/pipeline/deploy/metaflow_offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/deploy/offline_deploy.py` & `lolpop-0.1.0a9/lolpop/pipeline/deploy/offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/predict/metaflow_offline_predict.py` & `lolpop-0.1.0a9/lolpop/pipeline/predict/metaflow_offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/predict/offline_predict.py` & `lolpop-0.1.0a9/lolpop/pipeline/predict/offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/process/metaflow_offline_process.py` & `lolpop-0.1.0a9/lolpop/pipeline/process/metaflow_offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/process/offline_process.py` & `lolpop-0.1.0a9/lolpop/pipeline/process/offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/train/base_train.py` & `lolpop-0.1.0a9/lolpop/pipeline/train/base_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/train/metaflow_offline_train.py` & `lolpop-0.1.0a9/lolpop/pipeline/train/metaflow_offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/train/offline_train.py` & `lolpop-0.1.0a9/lolpop/pipeline/train/offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py` & `lolpop-0.1.0a9/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/runner/__init__.py` & `lolpop-0.1.0a9/lolpop/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/runner/base_runner.py` & `lolpop-0.1.0a9/lolpop/runner/base_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from lolpop.utils import common_utils as utils
 from inspect import currentframe
-
 class BaseRunner: 
 
     __REQUIRED_CONF__ = {
         "pipelines": [], 
         "components": ["metadata_tracker"], 
         "config": []
     }
@@ -15,14 +14,16 @@
     suppress_logger = False 
     suppress_notifier = False
 
     def __init__(self, conf={}, problem_type = "unspecified_problem_type", plugin_paths=[], 
                  skip_config_validation=False, *args, **kwargs):
         #handle configuration 
         self.name = type(self).__name__
+        self.type = self.__module__.split(".")[-2]
+        self.integration_type = self.__module__.split(".")[-1]
         conf = utils.get_conf(conf)
         conf = utils.resolve_conf_variables(conf)
         conf = utils.copy_config_into(conf, self.__DEFAULT_CONF__) 
         if not skip_config_validation:
             conf = self._validate_conf(conf)
         self.config = conf.get("config", {})
         self.problem_type = conf.get("problem_type", problem_type)
@@ -48,44 +49,25 @@
         ##    <key>: <value>
         # components can be defined at the runner or pipeline level and this determines the component scope.  
         # components defined at the runner level are passed down to all pipelines and components, 
         # so that they are globally acessible, whereas a component defined at the pipeline level are only accessible
         # in that pipeline and components defined at that pipeline. 
         # componenets in the right scope should know about each other but pipelines act independently (for now, at least)
 
-        #set up logger first because we want to pass that to all children
-        #we set this up separately from the other components in case you want access to the logger in the 
-        #__init__ function
-        logger_obj = utils.register_component_class(self, conf, "logger", default_class_name="StdOutLogger", 
-                                                    runner_conf = self.config, plugin_mods=plugin_mods, 
-                                                    skip_config_validation=skip_config_validation)
-        if logger_obj is not None: 
-            runner_components = {"logger" : logger_obj}
-            self.log("Loaded class %s into component %s" %(type(self.logger).__name__, "logger"))
-        else: 
-            raise Exception("Unable to find logger class.")
-
-        #we also want to special handle the metadata tracker, so we'll set that up first as well and pass 
-        #it to all children so they have access in __init__. 
-        #it's unclear why you might not want to use a metadata tracker, 
-        #but we sould consider this use case in the future 
-        meta_obj = utils.register_component_class(self, conf, "metadata_tracker", runner_conf=self.config, parent_process=self.name,
-                                                  problem_type=self.problem_type, dependent_components=runner_components, 
-                                                  plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
-        if meta_obj is not None:
-            runner_components["metadata_tracker"] = meta_obj
-            self.log("Loaded class %s into component %s" %(type(self.metadata_tracker).__name__, "metadata_tracker"))
-        else: 
-            #for local dev you may turn off metadata_tracker, so let's not strictly enforce that it exists for now
-            self.log("Unable to load metadata_tracker component.")
+        #handle default components: logger, notifier, metadata_tracker
+        runner_components = {}
+        runner_components = utils.set_up_default_components(self, conf, self.config,
+                                                            plugin_mods=plugin_mods, 
+                                                            skip_config_validation=skip_config_validation,
+                                                            components = runner_components)
 
         #build all other components
         for component in conf.get("components",{}).keys(): 
             #ignore logger and metadata_tracker since we have already set those up
-            if component != "logger" and component !="metadata_tracker": 
+            if component != "logger" and component !="metadata_tracker" and component !="notifier": 
                 obj = utils.register_component_class(self, conf, component, runner_conf=self.config, parent_process=self.name,
                                                      problem_type=self.problem_type, dependent_components=runner_components, 
                                                      plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
                 if obj is not None: 
                     self.log("Loaded class %s into component %s" %(type(getattr(self, component)).__name__, component))
                     runner_components[component] = obj
                 else:
```

### Comparing `lolpop-0.1.0a8/lolpop/runner/classification_runner/classification_runner.py` & `lolpop-0.1.0a9/lolpop/runner/classification_runner/classification_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/runner/classification_runner/metaflow_classification.py` & `lolpop-0.1.0a9/lolpop/runner/classification_runner/metaflow_classification.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/runner/timeseries_runner/timeseries_runner.py` & `lolpop-0.1.0a9/lolpop/runner/timeseries_runner/timeseries_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py` & `lolpop-0.1.0a9/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py` & `lolpop-0.1.0a9/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py` & `lolpop-0.1.0a9/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py` & `lolpop-0.1.0a9/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py` & `lolpop-0.1.0a9/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py` & `lolpop-0.1.0a9/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/utils/continual_utils.py` & `lolpop-0.1.0a9/lolpop/utils/continual_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/utils/metaflow_utils.py` & `lolpop-0.1.0a9/lolpop/utils/metaflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/lolpop/utils/mlflow_utils.py` & `lolpop-0.1.0a9/lolpop/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a8/pyproject.toml` & `lolpop-0.1.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lolpop"
-version = "v0.1.0-alpha.8"
+version = "v0.1.0-alpha.9"
 description = "A software engineering framework for machine learning workflows"
 authors = ["jordanvolz <jordan.volz@gmail.com>"]
 repository = "https://github.com/jordanvolz/lolpop"
 #hompage = 
 #documentation = 
 keywords = ["machine learning", "data science", "mlops"]
 license = "Apache-2.0"
```

### Comparing `lolpop-0.1.0a8/PKG-INFO` & `lolpop-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolpop
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: A software engineering framework for machine learning workflows
 Home-page: https://github.com/jordanvolz/lolpop
 License: Apache-2.0
 Keywords: machine learning,data science,mlops
 Author: jordanvolz
 Author-email: jordan.volz@gmail.com
 Requires-Python: >=3.9,<3.11
```

