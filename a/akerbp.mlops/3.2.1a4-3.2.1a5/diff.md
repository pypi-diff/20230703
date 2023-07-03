# Comparing `tmp/akerbp.mlops-3.2.1a4.tar.gz` & `tmp/akerbp.mlops-3.2.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-k9qwrm15/akerbp.mlops-3.2.1a4.tar", last modified: Thu Jun 29 10:57:27 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-pi4ck2bb/akerbp.mlops-3.2.1a5.tar", last modified: Mon Jul  3 13:12:01 2023, max compression
```

## Comparing `akerbp.mlops-3.2.1a4.tar` & `akerbp.mlops-3.2.1a5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.012882 akerbp.mlops-3.2.1a4/
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      324 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-29 10:57:27.012882 akerbp.mlops-3.2.1a4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35467 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     4303 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.004882 akerbp.mlops-3.2.1a4/bitbucket_pipeline_helpers/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/install.sh
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.004882 akerbp.mlops-3.2.1a4/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/model_artifact/mlpet_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.004882 akerbp.mlops-3.2.1a4/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     9932 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     5427 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-29 10:57:27.012882 akerbp.mlops-3.2.1a4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.000882 akerbp.mlops-3.2.1a4/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.000882 akerbp.mlops-3.2.1a4/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.004882 akerbp.mlops-3.2.1a4/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.004882 akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38715 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.008882 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16504 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.008882 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     5828 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21411 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.008882 akerbp.mlops-3.2.1a4/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22835 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.008882 akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8607 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.004882 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    48989 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2394 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-06-29 10:57:26.000000 akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.008882 akerbp.mlops-3.2.1a4/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-29 10:57:27.012882 akerbp.mlops-3.2.1a4/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3562 2023-06-29 10:57:06.000000 akerbp.mlops-3.2.1a4/test/test_version_increment.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      324 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35467 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.709831 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/bitbucket_pipeline_helpers/upload_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_artifact/mlpet_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     9932 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     5427 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.705831 akerbp.mlops-3.2.1a5/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.705831 akerbp.mlops-3.2.1a5/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38715 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.717831 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16504 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.717831 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5828 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21411 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.717831 akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22835 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8620 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.713832 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    48989 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-03 13:12:01.000000 akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-03 13:12:01.721832 akerbp.mlops-3.2.1a5/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3562 2023-07-03 13:11:39.000000 akerbp.mlops-3.2.1a5/test/test_version_increment.py
```

### Comparing `akerbp.mlops-3.2.1a4/.flake8` & `akerbp.mlops-3.2.1a5/.flake8`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/.pre-commit-config.yaml` & `akerbp.mlops-3.2.1a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/LICENSE` & `akerbp.mlops-3.2.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/PKG-INFO` & `akerbp.mlops-3.2.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a4
+Version: 3.2.1a5
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a4/README.md` & `akerbp.mlops-3.2.1a5/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a5/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/build.sh` & `akerbp.mlops-3.2.1a5/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/increment_package_version.py` & `akerbp.mlops-3.2.1a5/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/mlops_settings.yaml` & `akerbp.mlops-3.2.1a5/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/model_code/model.py` & `akerbp.mlops-3.2.1a5/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/model_code/test_model.py` & `akerbp.mlops-3.2.1a5/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/pyproject.toml` & `akerbp.mlops-3.2.1a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/prediction.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             mlops_helpers.client_secrets = secrets
             mlops_helpers.set_up_cdf_client(context="write")
         logger.info("Initializing model")
         initialization(secrets)
         logger.info("Model initialized")
 
         try:
-            skip_input_validation = eval(
+            skip_input_validation = ast.literal_eval(
                 c.info["prediction"]["metadata"]["supports_external_retrieval"]
             )
         except KeyError as e:
             raise MissingFieldError(
                 "Field 'supports_external_retrieval' is missing from the metadata specification in mlops_settings.yaml"
             ) from e
         if skip_input_validation:
@@ -101,14 +101,15 @@
         y = predict(data, init_object, secrets)  # type: ignore
         logger.info("Predictions obtained")
         write_predictions_to_file = data.get("return_file", False)
         if write_predictions_to_file:
             logger.info("Writing predictions to file")
             if platform == "cdf":
                 import base64
+
                 public_key = data.get("public_key", None)
                 content = str(json.dumps(y))
                 data_encrypted = False
                 if public_key is None:
                     logger.warning(
                         "Public key is not provided. The predictions will not be encrypted. This is not recommended!"
                     )
```

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.2.1a5/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.2.1a4
+Version: 3.2.1a5
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.2.1a4/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.2.1a5/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_data_validation.py` & `akerbp.mlops-3.2.1a5/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_install_requirements.py` & `akerbp.mlops-3.2.1a5/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_metadata_validation.py` & `akerbp.mlops-3.2.1a5/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.2.1a5/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.2.1a4/test/test_version_increment.py` & `akerbp.mlops-3.2.1a5/test/test_version_increment.py`

 * *Files identical despite different names*

