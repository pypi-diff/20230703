# Comparing `tmp/validio_sdk-0.5.1.tar.gz` & `tmp/validio_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_sdk-0.5.1.tar", max compression
+gzip compressed data, was "validio_sdk-0.6.0.tar", max compression
```

## Comparing `validio_sdk-0.5.1.tar` & `validio_sdk-0.6.0.tar`

### file list

```diff
@@ -1,202 +1,227 @@
--rw-r--r--   0        0        0    11340 2023-06-16 09:49:53.394037 validio_sdk-0.5.1/LICENSE
--rw-r--r--   0        0        0      308 2023-06-16 09:49:53.394037 validio_sdk-0.5.1/README_PUBLIC.md
--rw-r--r--   0        0        0     5010 2023-06-16 09:50:04.553826 validio_sdk-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      588 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/code/__init__.py
--rw-r--r--   0        0        0      551 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/code/apply.py
--rw-r--r--   0        0        0     4767 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/code/plan.py
--rw-r--r--   0        0        0     1565 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/code/scaffold.py
--rw-r--r--   0        0        0      305 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/code/settings.py
--rw-r--r--   0        0        0     5891 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/config.py
--rw-r--r--   0        0        0   245071 2023-06-16 09:49:53.398037 validio_sdk-0.5.1/validio_sdk/graphql_client/__init__.py
--rw-r--r--   0        0        0      573 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/apply_validator_recommendation.py
--rw-r--r--   0        0        0     7319 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      526 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/aws_credential_secret_changed.py
--rw-r--r--   0        0        0      613 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
--rw-r--r--   0        0        0      614 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/backfill_source.py
--rw-r--r--   0        0        0     1899 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/base_model.py
--rw-r--r--   0        0        0   584680 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/client.py
--rw-r--r--   0        0        0      445 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_credential.py
--rw-r--r--   0        0        0      528 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_kinesis_destination.py
--rw-r--r--   0        0        0      468 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_kinesis_source.py
--rw-r--r--   0        0        0      526 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_redshift_credential.py
--rw-r--r--   0        0        0      480 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_redshift_source.py
--rw-r--r--   0        0        0      418 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_s3_source.py
--rw-r--r--   0        0        0      843 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      823 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      455 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_demo_credential.py
--rw-r--r--   0        0        0      407 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_demo_source.py
--rw-r--r--   0        0        0      407 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_file_window.py
--rw-r--r--   0        0        0      468 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_fixed_batch_window.py
--rw-r--r--   0        0        0      702 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      682 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      539 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_big_query_destination.py
--rw-r--r--   0        0        0      481 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_big_query_source.py
--rw-r--r--   0        0        0      445 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_credential.py
--rw-r--r--   0        0        0      500 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      459 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      468 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_storage_source.py
--rw-r--r--   0        0        0      487 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_notification_rule.py
--rw-r--r--   0        0        0      753 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      803 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      783 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      823 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      682 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      662 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      702 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      516 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_postgre_sql_credential.py
--rw-r--r--   0        0        0      468 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_postgre_sql_source.py
--rw-r--r--   0        0        0      733 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      713 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      753 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      753 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      733 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      528 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_saml_identity_provider.py
--rw-r--r--   0        0        0      438 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_segmentation.py
--rw-r--r--   0        0        0      477 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_sessionized_window.py
--rw-r--r--   0        0        0      429 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_slack_channel.py
--rw-r--r--   0        0        0      505 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_snowflake_credential.py
--rw-r--r--   0        0        0      517 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_snowflake_destination.py
--rw-r--r--   0        0        0      457 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_snowflake_source.py
--rw-r--r--   0        0        0      447 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_tumbling_window.py
--rw-r--r--   0        0        0      328 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_user.py
--rw-r--r--   0        0        0      672 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0      652 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0      449 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/create_webhook_channel.py
--rw-r--r--   0        0        0      364 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_channel.py
--rw-r--r--   0        0        0      614 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_credential.py
--rw-r--r--   0        0        0      622 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_credentials.py
--rw-r--r--   0        0        0      630 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_destination.py
--rw-r--r--   0        0        0      638 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_destinations.py
--rw-r--r--   0        0        0      376 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_identity.py
--rw-r--r--   0        0        0      487 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_identity_provider.py
--rw-r--r--   0        0        0      487 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_notification_rule.py
--rw-r--r--   0        0        0      646 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_segmentation.py
--rw-r--r--   0        0        0      536 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_source.py
--rw-r--r--   0        0        0      544 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_sources.py
--rw-r--r--   0        0        0      328 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_user.py
--rw-r--r--   0        0        0      606 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_validators.py
--rw-r--r--   0        0        0      536 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_window.py
--rw-r--r--   0        0        0      544 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/delete_windows.py
--rw-r--r--   0        0        0      589 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/dismiss_validator_recommendation.py
--rw-r--r--   0        0        0     3065 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/enums.py
--rw-r--r--   0        0        0     2314 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/exceptions.py
--rw-r--r--   0        0        0   175196 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/fragments.py
--rw-r--r--   0        0        0      526 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/gcp_credential_secret_changed.py
--rw-r--r--   0        0        0     2896 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_channel_by_resource_name.py
--rw-r--r--   0        0        0     2427 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_channels.py
--rw-r--r--   0        0        0     4965 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_credential_by_resource_name.py
--rw-r--r--   0        0        0     5997 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_destination_by_resource_name.py
--rw-r--r--   0        0        0     2218 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
--rw-r--r--   0        0        0     2033 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_identity_providers.py
--rw-r--r--   0        0        0     5368 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_incidents.py
--rw-r--r--   0        0        0      627 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_notification_rules.py
--rw-r--r--   0        0        0      460 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_segment_incidents.py
--rw-r--r--   0        0        0      357 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_segmentation.py
--rw-r--r--   0        0        0      572 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
--rw-r--r--   0        0        0    20258 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_source.py
--rw-r--r--   0        0        0    24833 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_source_by_resource_name.py
--rw-r--r--   0        0        0     1727 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_source_incidents.py
--rw-r--r--   0        0        0    21532 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_source_recommended_validators.py
--rw-r--r--   0        0        0      476 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_user_by_resource_name.py
--rw-r--r--   0        0        0      300 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_users.py
--rw-r--r--   0        0        0    40168 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator.py
--rw-r--r--   0        0        0    48254 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_by_resource_name.py
--rw-r--r--   0        0        0      480 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_incidents.py
--rw-r--r--   0        0        0      551 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_segment_incidents.py
--rw-r--r--   0        0        0     3986 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_segment_metrics.py
--rw-r--r--   0        0        0     5711 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/get_window_by_resource_name.py
--rw-r--r--   0        0        0      290 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
--rw-r--r--   0        0        0      308 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_aws_redshift_schema.py
--rw-r--r--   0        0        0      270 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_aws_s3_schema.py
--rw-r--r--   0        0        0      265 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_demo_schema.py
--rw-r--r--   0        0        0      309 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
--rw-r--r--   0        0        0      318 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
--rw-r--r--   0        0        0      287 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
--rw-r--r--   0        0        0      290 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_gcp_storage_schema.py
--rw-r--r--   0        0        0      290 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_postgre_sql_schema.py
--rw-r--r--   0        0        0      285 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/infer_snowflake_schema.py
--rw-r--r--   0        0        0    34533 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/input_types.py
--rw-r--r--   0        0        0     4316 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/list_credentials.py
--rw-r--r--   0        0        0     5202 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/list_destinations.py
--rw-r--r--   0        0        0      457 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/list_segmentations.py
--rw-r--r--   0        0        0    21364 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/list_sources.py
--rw-r--r--   0        0        0    42237 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/list_validators.py
--rw-r--r--   0        0        0     4976 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/list_windows.py
--rw-r--r--   0        0        0      603 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
--rw-r--r--   0        0        0      594 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/scalars.py
--rw-r--r--   0        0        0      288 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/segments.py
--rw-r--r--   0        0        0      499 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/segments_by_resource_name.py
--rw-r--r--   0        0        0      592 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
--rw-r--r--   0        0        0      566 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/start_source.py
--rw-r--r--   0        0        0      550 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/stop_source.py
--rw-r--r--   0        0        0      441 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_credential.py
--rw-r--r--   0        0        0      524 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_kinesis_destination.py
--rw-r--r--   0        0        0      464 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_kinesis_source.py
--rw-r--r--   0        0        0      522 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_redshift_credential.py
--rw-r--r--   0        0        0      476 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_redshift_source.py
--rw-r--r--   0        0        0      414 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_s3_source.py
--rw-r--r--   0        0        0      636 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_categorical_distribution_validator.py
--rw-r--r--   0        0        0      464 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_fixed_batch_window.py
--rw-r--r--   0        0        0      491 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_freshness_validator.py
--rw-r--r--   0        0        0      535 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_big_query_destination.py
--rw-r--r--   0        0        0      477 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_big_query_source.py
--rw-r--r--   0        0        0      441 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_credential.py
--rw-r--r--   0        0        0      496 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
--rw-r--r--   0        0        0      455 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
--rw-r--r--   0        0        0      464 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_storage_source.py
--rw-r--r--   0        0        0      534 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_local_identity_provider.py
--rw-r--r--   0        0        0      483 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_notification_rule.py
--rw-r--r--   0        0        0      540 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
--rw-r--r--   0        0        0      596 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_numeric_distribution_validator.py
--rw-r--r--   0        0        0      469 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_numeric_validator.py
--rw-r--r--   0        0        0      512 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_postgre_sql_credential.py
--rw-r--r--   0        0        0      464 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_postgre_sql_source.py
--rw-r--r--   0        0        0      520 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_relative_time_validator.py
--rw-r--r--   0        0        0      540 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_relative_volume_validator.py
--rw-r--r--   0        0        0      524 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_saml_identity_provider.py
--rw-r--r--   0        0        0      473 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_sessionized_window.py
--rw-r--r--   0        0        0      425 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_slack_channel.py
--rw-r--r--   0        0        0      501 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_snowflake_credential.py
--rw-r--r--   0        0        0      513 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_snowflake_destination.py
--rw-r--r--   0        0        0      453 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_snowflake_source.py
--rw-r--r--   0        0        0      443 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_tumbling_window.py
--rw-r--r--   0        0        0      324 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_user.py
--rw-r--r--   0        0        0    57176 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
--rw-r--r--   0        0        0    56052 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
--rw-r--r--   0        0        0    58306 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
--rw-r--r--   0        0        0      459 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_volume_validator.py
--rw-r--r--   0        0        0      445 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/graphql_client/update_webhook_channel.py
--rw-r--r--   0        0        0      265 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/metadata.py
--rw-r--r--   0        0        0        0 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/py.typed
--rw-r--r--   0        0        0      135 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/resource/__init__.py
--rw-r--r--   0        0        0    21078 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/resource/_diff.py
--rw-r--r--   0        0        0     1208 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/resource/_diff_util.py
--rw-r--r--   0        0        0     1657 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/resource/_diffable.py
--rw-r--r--   0        0        0     1579 2023-06-16 09:49:53.402037 validio_sdk-0.5.1/validio_sdk/resource/_errors.py
--rw-r--r--   0        0        0     4002 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/_field_selector.py
--rw-r--r--   0        0        0    17790 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/_resource.py
--rw-r--r--   0        0        0     1355 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/_resource_graph.py
--rw-r--r--   0        0        0     5366 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/_serde.py
--rw-r--r--   0        0        0    21047 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/_server_resources.py
--rw-r--r--   0        0        0      847 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/_util.py
--rw-r--r--   0        0        0     5027 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/channels.py
--rw-r--r--   0        0        0     7692 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/credentials.py
--rw-r--r--   0        0        0     5398 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/destinations.py
--rw-r--r--   0        0        0     6255 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/filters.py
--rw-r--r--   0        0        0     4846 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/notification_rules.py
--rw-r--r--   0        0        0     2040 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/segmentations.py
--rw-r--r--   0        0        0    25856 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/sources.py
--rw-r--r--   0        0        0        0 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/tests/__init__.py
--rw-r--r--   0        0        0    15408 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/tests/test__diff.py
--rw-r--r--   0        0        0     1905 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/tests/test__field_selector.py
--rw-r--r--   0        0        0    16357 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/tests/test__resource.py
--rw-r--r--   0        0        0     5638 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/thresholds.py
--rw-r--r--   0        0        0    32563 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/validators.py
--rw-r--r--   0        0        0     5995 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/resource/windows.py
--rw-r--r--   0        0        0     1377 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/scalars.py
--rw-r--r--   0        0        0     1813 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/util.py
--rw-r--r--   0        0        0     2382 2023-06-16 09:49:53.406037 validio_sdk-0.5.1/validio_sdk/validio_client.py
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-07-03 15:11:56.619963 validio_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0      308 2023-07-03 15:11:56.619963 validio_sdk-0.6.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     5010 2023-07-03 15:12:08.951918 validio_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/__init__.py
+-rw-r--r--   0        0        0      551 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/apply.py
+-rw-r--r--   0        0        0     4767 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/plan.py
+-rw-r--r--   0        0        0     1565 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/scaffold.py
+-rw-r--r--   0        0        0      305 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/code/settings.py
+-rw-r--r--   0        0        0     5891 2023-07-03 15:11:56.623963 validio_sdk-0.6.0/validio_sdk/config.py
+-rw-r--r--   0        0        0   261486 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/apply_validator_recommendation.py
+-rw-r--r--   0        0        0     7319 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      526 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/aws_credential_secret_changed.py
+-rw-r--r--   0        0        0      613 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py
+-rw-r--r--   0        0        0      614 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/backfill_source.py
+-rw-r--r--   0        0        0     1899 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/base_model.py
+-rw-r--r--   0        0        0   654498 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/client.py
+-rw-r--r--   0        0        0      506 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_athena_credential.py
+-rw-r--r--   0        0        0      458 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_athena_source.py
+-rw-r--r--   0        0        0      445 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_credential.py
+-rw-r--r--   0        0        0      528 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_kinesis_source.py
+-rw-r--r--   0        0        0      526 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_redshift_credential.py
+-rw-r--r--   0        0        0      480 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_redshift_source.py
+-rw-r--r--   0        0        0      418 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_s3_source.py
+-rw-r--r--   0        0        0      843 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      455 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_demo_credential.py
+-rw-r--r--   0        0        0      407 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_demo_source.py
+-rw-r--r--   0        0        0      407 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_file_window.py
+-rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_fixed_batch_window.py
+-rw-r--r--   0        0        0      702 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      539 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      481 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_big_query_source.py
+-rw-r--r--   0        0        0      445 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_credential.py
+-rw-r--r--   0        0        0      500 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      459 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_storage_source.py
+-rw-r--r--   0        0        0      557 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_sasl_plain_credential.py
+-rw-r--r--   0        0        0      417 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_source.py
+-rw-r--r--   0        0        0      498 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      487 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_notification_rule.py
+-rw-r--r--   0        0        0      753 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      803 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      783 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      823 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      682 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      662 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      702 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      516 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_postgre_sql_credential.py
+-rw-r--r--   0        0        0      468 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_postgre_sql_source.py
+-rw-r--r--   0        0        0      733 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      713 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      753 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      733 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      528 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_saml_identity_provider.py
+-rw-r--r--   0        0        0      438 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_segmentation.py
+-rw-r--r--   0        0        0      477 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_sessionized_window.py
+-rw-r--r--   0        0        0      429 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_slack_channel.py
+-rw-r--r--   0        0        0      505 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_credential.py
+-rw-r--r--   0        0        0      517 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_destination.py
+-rw-r--r--   0        0        0      457 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_source.py
+-rw-r--r--   0        0        0      447 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_tumbling_window.py
+-rw-r--r--   0        0        0      328 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_user.py
+-rw-r--r--   0        0        0      672 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0      652 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0      449 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/create_webhook_channel.py
+-rw-r--r--   0        0        0      364 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_channel.py
+-rw-r--r--   0        0        0      614 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credential.py
+-rw-r--r--   0        0        0      622 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credentials.py
+-rw-r--r--   0        0        0      630 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destination.py
+-rw-r--r--   0        0        0      638 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destinations.py
+-rw-r--r--   0        0        0      376 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_identity.py
+-rw-r--r--   0        0        0      487 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_identity_provider.py
+-rw-r--r--   0        0        0      487 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_notification_rule.py
+-rw-r--r--   0        0        0      646 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_segmentation.py
+-rw-r--r--   0        0        0      536 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_source.py
+-rw-r--r--   0        0        0      544 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_sources.py
+-rw-r--r--   0        0        0      328 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_user.py
+-rw-r--r--   0        0        0      606 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_validators.py
+-rw-r--r--   0        0        0      536 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_window.py
+-rw-r--r--   0        0        0      544 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/delete_windows.py
+-rw-r--r--   0        0        0      589 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py
+-rw-r--r--   0        0        0     3127 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/enums.py
+-rw-r--r--   0        0        0     2314 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/exceptions.py
+-rw-r--r--   0        0        0   188660 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/fragments.py
+-rw-r--r--   0        0        0      526 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py
+-rw-r--r--   0        0        0     2896 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_channel_by_resource_name.py
+-rw-r--r--   0        0        0     2427 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_channels.py
+-rw-r--r--   0        0        0     8124 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_credential_by_resource_name.py
+-rw-r--r--   0        0        0     5997 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_destination_by_resource_name.py
+-rw-r--r--   0        0        0     2218 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py
+-rw-r--r--   0        0        0     2033 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_providers.py
+-rw-r--r--   0        0        0     5368 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_incidents.py
+-rw-r--r--   0        0        0      627 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_notification_rules.py
+-rw-r--r--   0        0        0     2245 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_recommendation.py
+-rw-r--r--   0        0        0      460 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_segment_incidents.py
+-rw-r--r--   0        0        0      357 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_segmentation.py
+-rw-r--r--   0        0        0      572 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py
+-rw-r--r--   0        0        0    23998 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source.py
+-rw-r--r--   0        0        0    29447 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_by_resource_name.py
+-rw-r--r--   0        0        0     1727 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_incidents.py
+-rw-r--r--   0        0        0    25201 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_recommended_validators.py
+-rw-r--r--   0        0        0      476 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_user_by_resource_name.py
+-rw-r--r--   0        0        0      300 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_users.py
+-rw-r--r--   0        0        0    40168 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator.py
+-rw-r--r--   0        0        0    48254 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_by_resource_name.py
+-rw-r--r--   0        0        0      480 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_incidents.py
+-rw-r--r--   0        0        0      551 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_incidents.py
+-rw-r--r--   0        0        0     3986 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_metrics.py
+-rw-r--r--   0        0        0     5711 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/get_window_by_resource_name.py
+-rw-r--r--   0        0        0      286 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_athena_schema.py
+-rw-r--r--   0        0        0      290 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_kinesis_schema.py
+-rw-r--r--   0        0        0      308 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_redshift_schema.py
+-rw-r--r--   0        0        0      270 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_aws_s3_schema.py
+-rw-r--r--   0        0        0      265 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_demo_schema.py
+-rw-r--r--   0        0        0      309 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_big_query_schema.py
+-rw-r--r--   0        0        0      318 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_pub_sub_lite_schema.py
+-rw-r--r--   0        0        0      287 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_pub_sub_schema.py
+-rw-r--r--   0        0        0      290 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_gcp_storage_schema.py
+-rw-r--r--   0        0        0      269 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_kafka_schema.py
+-rw-r--r--   0        0        0      290 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_postgre_sql_schema.py
+-rw-r--r--   0        0        0      285 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/infer_snowflake_schema.py
+-rw-r--r--   0        0        0    39472 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/input_types.py
+-rw-r--r--   0        0        0      644 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/kafka_sasl_plain_credential_secret_changed.py
+-rw-r--r--   0        0        0      583 2023-07-03 15:11:56.627963 validio_sdk-0.6.0/validio_sdk/graphql_client/kafka_ssl_credential_secret_changed.py
+-rw-r--r--   0        0        0     7067 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_credentials.py
+-rw-r--r--   0        0        0     5202 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_destinations.py
+-rw-r--r--   0        0        0      457 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_segmentations.py
+-rw-r--r--   0        0        0    25314 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_sources.py
+-rw-r--r--   0        0        0    42237 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_validators.py
+-rw-r--r--   0        0        0     4976 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/list_windows.py
+-rw-r--r--   0        0        0      603 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py
+-rw-r--r--   0        0        0      594 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/scalars.py
+-rw-r--r--   0        0        0      288 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/segments.py
+-rw-r--r--   0        0        0      499 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/segments_by_resource_name.py
+-rw-r--r--   0        0        0      592 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py
+-rw-r--r--   0        0        0      566 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/start_source.py
+-rw-r--r--   0        0        0      550 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/stop_source.py
+-rw-r--r--   0        0        0      502 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_athena_credential.py
+-rw-r--r--   0        0        0      454 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_athena_source.py
+-rw-r--r--   0        0        0      441 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_credential.py
+-rw-r--r--   0        0        0      524 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py
+-rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_kinesis_source.py
+-rw-r--r--   0        0        0      522 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_redshift_credential.py
+-rw-r--r--   0        0        0      476 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_redshift_source.py
+-rw-r--r--   0        0        0      414 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_s3_source.py
+-rw-r--r--   0        0        0      636 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_channel_namespace.py
+-rw-r--r--   0        0        0      499 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_credential_namespace.py
+-rw-r--r--   0        0        0      509 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_destination_namespace.py
+-rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_fixed_batch_window.py
+-rw-r--r--   0        0        0      491 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_freshness_validator.py
+-rw-r--r--   0        0        0      535 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py
+-rw-r--r--   0        0        0      477 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_big_query_source.py
+-rw-r--r--   0        0        0      441 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_credential.py
+-rw-r--r--   0        0        0      496 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_pub_sub_lite_source.py
+-rw-r--r--   0        0        0      455 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_pub_sub_source.py
+-rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_storage_source.py
+-rw-r--r--   0        0        0      560 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_identity_provider_namespace.py
+-rw-r--r--   0        0        0      553 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_sasl_plain_credential.py
+-rw-r--r--   0        0        0      413 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_source.py
+-rw-r--r--   0        0        0      494 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_kafka_ssl_credential.py
+-rw-r--r--   0        0        0      534 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_local_identity_provider.py
+-rw-r--r--   0        0        0      483 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_notification_rule.py
+-rw-r--r--   0        0        0      560 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_notification_rule_namespace.py
+-rw-r--r--   0        0        0      540 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py
+-rw-r--r--   0        0        0      596 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py
+-rw-r--r--   0        0        0      469 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_validator.py
+-rw-r--r--   0        0        0      512 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_postgre_sql_credential.py
+-rw-r--r--   0        0        0      464 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_postgre_sql_source.py
+-rw-r--r--   0        0        0      520 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_time_validator.py
+-rw-r--r--   0        0        0      540 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_volume_validator.py
+-rw-r--r--   0        0        0      524 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_saml_identity_provider.py
+-rw-r--r--   0        0        0      519 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_segmentation_namespace.py
+-rw-r--r--   0        0        0      473 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_sessionized_window.py
+-rw-r--r--   0        0        0      425 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_slack_channel.py
+-rw-r--r--   0        0        0      501 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_credential.py
+-rw-r--r--   0        0        0      513 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_destination.py
+-rw-r--r--   0        0        0      453 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_source.py
+-rw-r--r--   0        0        0      459 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_source_namespace.py
+-rw-r--r--   0        0        0      443 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_tumbling_window.py
+-rw-r--r--   0        0        0      324 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_user.py
+-rw-r--r--   0        0        0      439 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_user_namespace.py
+-rw-r--r--   0        0        0      491 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_namespace.py
+-rw-r--r--   0        0        0    57176 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py
+-rw-r--r--   0        0        0    56052 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py
+-rw-r--r--   0        0        0    58306 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py
+-rw-r--r--   0        0        0      459 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_volume_validator.py
+-rw-r--r--   0        0        0      445 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_webhook_channel.py
+-rw-r--r--   0        0        0      459 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/graphql_client/update_window_namespace.py
+-rw-r--r--   0        0        0      265 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/metadata.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/py.typed
+-rw-r--r--   0        0        0      135 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/__init__.py
+-rw-r--r--   0        0        0    21078 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_diff.py
+-rw-r--r--   0        0        0     1505 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_diff_util.py
+-rw-r--r--   0        0        0     1657 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_diffable.py
+-rw-r--r--   0        0        0     1579 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_errors.py
+-rw-r--r--   0        0        0     4002 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_field_selector.py
+-rw-r--r--   0        0        0    17790 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_resource.py
+-rw-r--r--   0        0        0     1355 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_resource_graph.py
+-rw-r--r--   0        0        0     5366 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_serde.py
+-rw-r--r--   0        0        0    21679 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_server_resources.py
+-rw-r--r--   0        0        0      847 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/_util.py
+-rw-r--r--   0        0        0     5027 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/channels.py
+-rw-r--r--   0        0        0     7692 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/credentials.py
+-rw-r--r--   0        0        0     5601 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/destinations.py
+-rw-r--r--   0        0        0     6262 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/filters.py
+-rw-r--r--   0        0        0     4846 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/notification_rules.py
+-rw-r--r--   0        0        0     2040 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/segmentations.py
+-rw-r--r--   0        0        0    25888 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/sources.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/__init__.py
+-rw-r--r--   0        0        0    15408 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/test__diff.py
+-rw-r--r--   0        0        0     1905 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/test__field_selector.py
+-rw-r--r--   0        0        0    16357 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/tests/test__resource.py
+-rw-r--r--   0        0        0     5638 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/thresholds.py
+-rw-r--r--   0        0        0    32563 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/validators.py
+-rw-r--r--   0        0        0     5995 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/resource/windows.py
+-rw-r--r--   0        0        0     1377 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/scalars.py
+-rw-r--r--   0        0        0     1813 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/util.py
+-rw-r--r--   0        0        0     2382 2023-07-03 15:11:56.631963 validio_sdk-0.6.0/validio_sdk/validio_client.py
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 validio_sdk-0.6.0/PKG-INFO
```

### Comparing `validio_sdk-0.5.1/LICENSE` & `validio_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/pyproject.toml` & `validio_sdk-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-sdk"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.5.1"
+version = "0.6.0"
 description = "SDK to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://dev.validio.io/sdk-docs"
 packages = [{ include = "validio_sdk" }]
 exclude = ["./validio_sdk/bin/pull_graphql.py", "./schema/**", "./plugins/**", "./examples/**"]
```

### Comparing `validio_sdk-0.5.1/validio_sdk/__init__.py` & `validio_sdk-0.6.0/validio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/code/apply.py` & `validio_sdk-0.6.0/validio_sdk/code/apply.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/code/plan.py` & `validio_sdk-0.6.0/validio_sdk/code/plan.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/code/scaffold.py` & `validio_sdk-0.6.0/validio_sdk/code/scaffold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/config.py` & `validio_sdk-0.6.0/validio_sdk/config.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/__init__.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 from .backfill_source import (
     BackfillSource,
     BackfillSourceSourceBackfill,
     BackfillSourceSourceBackfillErrors,
 )
 from .base_model import BaseModel
 from .client import Client
+from .create_aws_athena_credential import (
+    CreateAwsAthenaCredential,
+    CreateAwsAthenaCredentialAwsAthenaCredentialCreate,
+)
+from .create_aws_athena_source import (
+    CreateAwsAthenaSource,
+    CreateAwsAthenaSourceAwsAthenaSourceCreate,
+)
 from .create_aws_credential import (
     CreateAwsCredential,
     CreateAwsCredentialAwsCredentialCreate,
 )
 from .create_aws_kinesis_destination import (
     CreateAwsKinesisDestination,
     CreateAwsKinesisDestinationAwsKinesisDestinationCreate,
@@ -85,14 +93,23 @@
     CreateGcpPubSubSource,
     CreateGcpPubSubSourceGcpPubSubSourceCreate,
 )
 from .create_gcp_storage_source import (
     CreateGcpStorageSource,
     CreateGcpStorageSourceGcpStorageSourceCreate,
 )
+from .create_kafka_sasl_plain_credential import (
+    CreateKafkaSaslPlainCredential,
+    CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate,
+)
+from .create_kafka_source import CreateKafkaSource, CreateKafkaSourceKafkaSourceCreate
+from .create_kafka_ssl_credential import (
+    CreateKafkaSslCredential,
+    CreateKafkaSslCredentialKafkaSslCredentialCreate,
+)
 from .create_notification_rule import (
     CreateNotificationRule,
     CreateNotificationRuleNotificationRuleCreate,
 )
 from .create_numeric_anomaly_validator_with_dynamic_threshold import (
     CreateNumericAnomalyValidatorWithDynamicThreshold,
     CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate,
@@ -310,32 +327,44 @@
     ChannelUpdateChannelChannel,
     ChannelUpdateChannelSlackChannel,
     ChannelUpdateChannelSlackChannelConfig,
     ChannelUpdateChannelWebhookChannel,
     ChannelUpdateChannelWebhookChannelConfig,
     ChannelUpdateErrors,
     CredentialCreation,
+    CredentialCreationCredentialAwsAthenaCredential,
+    CredentialCreationCredentialAwsAthenaCredentialConfig,
     CredentialCreationCredentialAwsCredential,
     CredentialCreationCredentialAwsCredentialConfig,
     CredentialCreationCredentialAwsRedshiftCredential,
     CredentialCreationCredentialAwsRedshiftCredentialConfig,
     CredentialCreationCredentialCredential,
+    CredentialCreationCredentialKafkaSASLPlainCredential,
+    CredentialCreationCredentialKafkaSASLPlainCredentialConfig,
+    CredentialCreationCredentialKafkaSSLCredential,
+    CredentialCreationCredentialKafkaSSLCredentialConfig,
     CredentialCreationCredentialPostgreSqlCredential,
     CredentialCreationCredentialPostgreSqlCredentialConfig,
     CredentialCreationCredentialSnowflakeCredential,
     CredentialCreationCredentialSnowflakeCredentialConfig,
     CredentialCreationErrors,
     CredentialSecretChanged,
     CredentialSecretChangedErrors,
     CredentialUpdate,
+    CredentialUpdateCredentialAwsAthenaCredential,
+    CredentialUpdateCredentialAwsAthenaCredentialConfig,
     CredentialUpdateCredentialAwsCredential,
     CredentialUpdateCredentialAwsCredentialConfig,
     CredentialUpdateCredentialAwsRedshiftCredential,
     CredentialUpdateCredentialAwsRedshiftCredentialConfig,
     CredentialUpdateCredentialCredential,
+    CredentialUpdateCredentialKafkaSASLPlainCredential,
+    CredentialUpdateCredentialKafkaSASLPlainCredentialConfig,
+    CredentialUpdateCredentialKafkaSSLCredential,
+    CredentialUpdateCredentialKafkaSSLCredentialConfig,
     CredentialUpdateCredentialPostgreSqlCredential,
     CredentialUpdateCredentialPostgreSqlCredentialConfig,
     CredentialUpdateCredentialSnowflakeCredential,
     CredentialUpdateCredentialSnowflakeCredentialConfig,
     CredentialUpdateErrors,
     DeletedEntity,
     DestinationCreation,
@@ -375,14 +404,16 @@
     IdentityProviderDeletion,
     IdentityProviderDeletionErrors,
     IdentityProviderUpdate,
     IdentityProviderUpdateErrors,
     IdentityProviderUpdateIdentityProviderIdentityProvider,
     IdentityProviderUpdateIdentityProviderSamlIdentityProvider,
     IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig,
+    NamespaceUpdate,
+    NamespaceUpdateErrors,
     NotificationRuleCreation,
     NotificationRuleCreationErrors,
     NotificationRuleCreationNotificationRule,
     NotificationRuleDeletion,
     NotificationRuleDeletionErrors,
     NotificationRuleDeletionNotificationRule,
     NotificationRuleDetails,
@@ -403,14 +434,19 @@
     SegmentationDetails,
     SegmentationDetailsSource,
     SegmentationSummary,
     SegmentDetails,
     SegmentDetailsFields,
     SourceCreation,
     SourceCreationErrors,
+    SourceCreationSourceAwsAthenaSource,
+    SourceCreationSourceAwsAthenaSourceConfig,
+    SourceCreationSourceAwsAthenaSourceCredential,
+    SourceCreationSourceAwsAthenaSourceSegmentations,
+    SourceCreationSourceAwsAthenaSourceWindows,
     SourceCreationSourceAwsKinesisSource,
     SourceCreationSourceAwsKinesisSourceConfig,
     SourceCreationSourceAwsKinesisSourceCredential,
     SourceCreationSourceAwsKinesisSourceSegmentations,
     SourceCreationSourceAwsKinesisSourceWindows,
     SourceCreationSourceAwsRedshiftSource,
     SourceCreationSourceAwsRedshiftSourceConfig,
@@ -440,14 +476,19 @@
     SourceCreationSourceGcpPubSubSourceWindows,
     SourceCreationSourceGcpStorageSource,
     SourceCreationSourceGcpStorageSourceConfig,
     SourceCreationSourceGcpStorageSourceConfigCsv,
     SourceCreationSourceGcpStorageSourceCredential,
     SourceCreationSourceGcpStorageSourceSegmentations,
     SourceCreationSourceGcpStorageSourceWindows,
+    SourceCreationSourceKafkaSource,
+    SourceCreationSourceKafkaSourceConfig,
+    SourceCreationSourceKafkaSourceCredential,
+    SourceCreationSourceKafkaSourceSegmentations,
+    SourceCreationSourceKafkaSourceWindows,
     SourceCreationSourcePostgreSqlSource,
     SourceCreationSourcePostgreSqlSourceConfig,
     SourceCreationSourcePostgreSqlSourceCredential,
     SourceCreationSourcePostgreSqlSourceSegmentations,
     SourceCreationSourcePostgreSqlSourceWindows,
     SourceCreationSourceSnowflakeSource,
     SourceCreationSourceSnowflakeSourceConfig,
@@ -456,14 +497,19 @@
     SourceCreationSourceSnowflakeSourceWindows,
     SourceCreationSourceSource,
     SourceCreationSourceSourceCredential,
     SourceCreationSourceSourceSegmentations,
     SourceCreationSourceSourceWindows,
     SourceUpdate,
     SourceUpdateErrors,
+    SourceUpdateSourceAwsAthenaSource,
+    SourceUpdateSourceAwsAthenaSourceConfig,
+    SourceUpdateSourceAwsAthenaSourceCredential,
+    SourceUpdateSourceAwsAthenaSourceSegmentations,
+    SourceUpdateSourceAwsAthenaSourceWindows,
     SourceUpdateSourceAwsKinesisSource,
     SourceUpdateSourceAwsKinesisSourceConfig,
     SourceUpdateSourceAwsKinesisSourceCredential,
     SourceUpdateSourceAwsKinesisSourceSegmentations,
     SourceUpdateSourceAwsKinesisSourceWindows,
     SourceUpdateSourceAwsRedshiftSource,
     SourceUpdateSourceAwsRedshiftSourceConfig,
@@ -493,14 +539,19 @@
     SourceUpdateSourceGcpPubSubSourceWindows,
     SourceUpdateSourceGcpStorageSource,
     SourceUpdateSourceGcpStorageSourceConfig,
     SourceUpdateSourceGcpStorageSourceConfigCsv,
     SourceUpdateSourceGcpStorageSourceCredential,
     SourceUpdateSourceGcpStorageSourceSegmentations,
     SourceUpdateSourceGcpStorageSourceWindows,
+    SourceUpdateSourceKafkaSource,
+    SourceUpdateSourceKafkaSourceConfig,
+    SourceUpdateSourceKafkaSourceCredential,
+    SourceUpdateSourceKafkaSourceSegmentations,
+    SourceUpdateSourceKafkaSourceWindows,
     SourceUpdateSourcePostgreSqlSource,
     SourceUpdateSourcePostgreSqlSourceConfig,
     SourceUpdateSourcePostgreSqlSourceCredential,
     SourceUpdateSourcePostgreSqlSourceSegmentations,
     SourceUpdateSourcePostgreSqlSourceWindows,
     SourceUpdateSourceSnowflakeSource,
     SourceUpdateSourceSnowflakeSourceConfig,
@@ -764,19 +815,25 @@
     GetChannelsChannelsSlackChannel,
     GetChannelsChannelsSlackChannelConfig,
     GetChannelsChannelsWebhookChannel,
     GetChannelsChannelsWebhookChannelConfig,
 )
 from .get_credential_by_resource_name import (
     GetCredentialByResourceName,
+    GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential,
+    GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameAwsCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential,
     GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredentialConfig,
     GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential,
     GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig,
 )
 from .get_destination_by_resource_name import (
     GetDestinationByResourceName,
@@ -821,25 +878,37 @@
     GetNotificationRuleByResourceName,
     GetNotificationRuleByResourceNameNotificationRuleByResourceName,
 )
 from .get_notification_rules import (
     GetNotificationRules,
     GetNotificationRulesNotificationRules,
 )
+from .get_recommendation import (
+    GetRecommendation,
+    GetRecommendationRecommendationRecommendation,
+    GetRecommendationRecommendationValidatorCreateRecommendation,
+    GetRecommendationRecommendationValidatorDeleteRecommendation,
+    GetRecommendationRecommendationValidatorUpdateRecommendation,
+)
 from .get_segment_incidents import (
     GetSegmentIncidents,
     GetSegmentIncidentsSegmentIncidents,
 )
 from .get_segmentation import GetSegmentation, GetSegmentationSegmentation
 from .get_segmentation_by_resource_name import (
     GetSegmentationByResourceName,
     GetSegmentationByResourceNameSegmentationByResourceName,
 )
 from .get_source import (
     GetSource,
+    GetSourceSourceAwsAthenaSource,
+    GetSourceSourceAwsAthenaSourceConfig,
+    GetSourceSourceAwsAthenaSourceCredential,
+    GetSourceSourceAwsAthenaSourceSegmentations,
+    GetSourceSourceAwsAthenaSourceWindows,
     GetSourceSourceAwsKinesisSource,
     GetSourceSourceAwsKinesisSourceConfig,
     GetSourceSourceAwsKinesisSourceCredential,
     GetSourceSourceAwsKinesisSourceSegmentations,
     GetSourceSourceAwsKinesisSourceWindows,
     GetSourceSourceAwsRedshiftSource,
     GetSourceSourceAwsRedshiftSourceConfig,
@@ -869,14 +938,19 @@
     GetSourceSourceGcpPubSubSourceWindows,
     GetSourceSourceGcpStorageSource,
     GetSourceSourceGcpStorageSourceConfig,
     GetSourceSourceGcpStorageSourceConfigCsv,
     GetSourceSourceGcpStorageSourceCredential,
     GetSourceSourceGcpStorageSourceSegmentations,
     GetSourceSourceGcpStorageSourceWindows,
+    GetSourceSourceKafkaSource,
+    GetSourceSourceKafkaSourceConfig,
+    GetSourceSourceKafkaSourceCredential,
+    GetSourceSourceKafkaSourceSegmentations,
+    GetSourceSourceKafkaSourceWindows,
     GetSourceSourcePostgreSqlSource,
     GetSourceSourcePostgreSqlSourceConfig,
     GetSourceSourcePostgreSqlSourceCredential,
     GetSourceSourcePostgreSqlSourceSegmentations,
     GetSourceSourcePostgreSqlSourceWindows,
     GetSourceSourceSnowflakeSource,
     GetSourceSourceSnowflakeSourceConfig,
@@ -886,14 +960,19 @@
     GetSourceSourceSource,
     GetSourceSourceSourceCredential,
     GetSourceSourceSourceSegmentations,
     GetSourceSourceSourceWindows,
 )
 from .get_source_by_resource_name import (
     GetSourceByResourceName,
+    GetSourceByResourceNameSourceByResourceNameAwsAthenaSource,
+    GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceConfig,
+    GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceCredential,
+    GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceSegmentations,
+    GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceWindows,
     GetSourceByResourceNameSourceByResourceNameAwsKinesisSource,
     GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceConfig,
     GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceCredential,
     GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceSegmentations,
     GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceWindows,
     GetSourceByResourceNameSourceByResourceNameAwsRedshiftSource,
     GetSourceByResourceNameSourceByResourceNameAwsRedshiftSourceConfig,
@@ -923,14 +1002,19 @@
     GetSourceByResourceNameSourceByResourceNameGcpPubSubSourceWindows,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSource,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSourceConfig,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSourceConfigCsv,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSourceCredential,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSourceSegmentations,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSourceWindows,
+    GetSourceByResourceNameSourceByResourceNameKafkaSource,
+    GetSourceByResourceNameSourceByResourceNameKafkaSourceConfig,
+    GetSourceByResourceNameSourceByResourceNameKafkaSourceCredential,
+    GetSourceByResourceNameSourceByResourceNameKafkaSourceSegmentations,
+    GetSourceByResourceNameSourceByResourceNameKafkaSourceWindows,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSource,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceConfig,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceCredential,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceSegmentations,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceWindows,
     GetSourceByResourceNameSourceByResourceNameSnowflakeSource,
     GetSourceByResourceNameSourceByResourceNameSnowflakeSourceConfig,
@@ -953,55 +1037,63 @@
     GetSourceRecommendedValidatorsSource,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorStats,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidator,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorProgress,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfig,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSegmentation,
     GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSource,
+    GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorStats,
 )
 from .get_user_by_resource_name import (
     GetUserByResourceName,
     GetUserByResourceNameUserByResourceName,
 )
 from .get_users import GetUsers, GetUsersUsers
 from .get_validator import (
@@ -1219,25 +1311,32 @@
     GetWindowByResourceNameWindowByResourceNameSessionizedWindowSource,
     GetWindowByResourceNameWindowByResourceNameTumblingWindow,
     GetWindowByResourceNameWindowByResourceNameTumblingWindowConfig,
     GetWindowByResourceNameWindowByResourceNameTumblingWindowSource,
     GetWindowByResourceNameWindowByResourceNameWindow,
     GetWindowByResourceNameWindowByResourceNameWindowSource,
 )
+from .infer_aws_athena_schema import InferAwsAthenaSchema
 from .infer_aws_kinesis_schema import InferAwsKinesisSchema
 from .infer_aws_redshift_schema import InferAwsRedshiftSchema
 from .infer_aws_s3_schema import InferAwsS3Schema
 from .infer_demo_schema import InferDemoSchema
 from .infer_gcp_big_query_schema import InferGcpBigQuerySchema
 from .infer_gcp_pub_sub_lite_schema import InferGcpPubSubLiteSchema
 from .infer_gcp_pub_sub_schema import InferGcpPubSubSchema
 from .infer_gcp_storage_schema import InferGcpStorageSchema
+from .infer_kafka_schema import InferKafkaSchema
 from .infer_postgre_sql_schema import InferPostgreSqlSchema
 from .infer_snowflake_schema import InferSnowflakeSchema
 from .input_types import (
+    AwsAthenaCredentialCreateInput,
+    AwsAthenaCredentialUpdateInput,
+    AwsAthenaInferSchemaInput,
+    AwsAthenaSourceCreateInput,
+    AwsAthenaSourceUpdateInput,
     AwsCredentialCreateInput,
     AwsCredentialSecretChangedInput,
     AwsCredentialUpdateInput,
     AwsKinesisDestinationCreateInput,
     AwsKinesisDestinationUpdateInput,
     AwsKinesisInferSchemaInput,
     AwsKinesisSourceCreateInput,
@@ -1280,14 +1379,23 @@
     GcpPubSubSourceUpdateInput,
     GcpStorageInferSchemaInput,
     GcpStorageSourceCreateInput,
     GcpStorageSourceUpdateInput,
     IdentityDeleteInput,
     IdentityProviderDeleteInput,
     IncidentsInput,
+    KafkaInferSchemaInput,
+    KafkaSASLPlainCredentialCreateInput,
+    KafkaSASLPlainCredentialSecretChangedInput,
+    KafkaSASLPlainCredentialUpdateInput,
+    KafkaSourceCreateInput,
+    KafkaSourceUpdateInput,
+    KafkaSSLCredentialCreateInput,
+    KafkaSSLCredentialSecretChangedInput,
+    KafkaSSLCredentialUpdateInput,
     LocalIdentityProviderUpdateInput,
     MonotonicThresholdCreateInput,
     NotificationRuleCreateInput,
     NotificationRuleDeleteInput,
     NotificationRuleUpdateInput,
     NumericAnomalyValidatorCreateInput,
     NumericAnomalyValidatorUpdateInput,
@@ -1304,14 +1412,15 @@
     ReferenceSourceConfigCreateInput,
     ReferenceSourceConfigUpdateInput,
     RelativeTimeValidatorCreateInput,
     RelativeTimeValidatorUpdateInput,
     RelativeVolumeValidatorCreateInput,
     RelativeVolumeValidatorUpdateInput,
     ResourceFilter,
+    ResourceNamespaceUpdateInput,
     SamlIdentityProviderCreateInput,
     SamlIdentityProviderUpdateInput,
     SegmentationCreateInput,
     SegmentIncidentsInput,
     SessionizedWindowCreateInput,
     SessionizedWindowUpdateInput,
     SlackChannelCreateInput,
@@ -1342,21 +1451,35 @@
     ValidatorWithFixedThresholdUpdateInput,
     ValidatorWithMonotonicThresholdUpdateInput,
     VolumeValidatorCreateInput,
     VolumeValidatorUpdateInput,
     WebhookChannelCreateInput,
     WebhookChannelUpdateInput,
 )
+from .kafka_sasl_plain_credential_secret_changed import (
+    KafkaSaslPlainCredentialSecretChanged,
+    KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged,
+)
+from .kafka_ssl_credential_secret_changed import (
+    KafkaSslCredentialSecretChanged,
+    KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged,
+)
 from .list_credentials import (
     ListCredentials,
+    ListCredentialsCredentialsListAwsAthenaCredential,
+    ListCredentialsCredentialsListAwsAthenaCredentialConfig,
     ListCredentialsCredentialsListAwsCredential,
     ListCredentialsCredentialsListAwsCredentialConfig,
     ListCredentialsCredentialsListAwsRedshiftCredential,
     ListCredentialsCredentialsListAwsRedshiftCredentialConfig,
     ListCredentialsCredentialsListCredential,
+    ListCredentialsCredentialsListKafkaSASLPlainCredential,
+    ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig,
+    ListCredentialsCredentialsListKafkaSSLCredential,
+    ListCredentialsCredentialsListKafkaSSLCredentialConfig,
     ListCredentialsCredentialsListPostgreSqlCredential,
     ListCredentialsCredentialsListPostgreSqlCredentialConfig,
     ListCredentialsCredentialsListSnowflakeCredential,
     ListCredentialsCredentialsListSnowflakeCredentialConfig,
 )
 from .list_destinations import (
     ListDestinations,
@@ -1371,14 +1494,19 @@
     ListDestinationsDestinationsListSnowflakeDestination,
     ListDestinationsDestinationsListSnowflakeDestinationConfig,
     ListDestinationsDestinationsListSnowflakeDestinationCredential,
 )
 from .list_segmentations import ListSegmentations, ListSegmentationsSegmentationsList
 from .list_sources import (
     ListSources,
+    ListSourcesSourcesListAwsAthenaSource,
+    ListSourcesSourcesListAwsAthenaSourceConfig,
+    ListSourcesSourcesListAwsAthenaSourceCredential,
+    ListSourcesSourcesListAwsAthenaSourceSegmentations,
+    ListSourcesSourcesListAwsAthenaSourceWindows,
     ListSourcesSourcesListAwsKinesisSource,
     ListSourcesSourcesListAwsKinesisSourceConfig,
     ListSourcesSourcesListAwsKinesisSourceCredential,
     ListSourcesSourcesListAwsKinesisSourceSegmentations,
     ListSourcesSourcesListAwsKinesisSourceWindows,
     ListSourcesSourcesListAwsRedshiftSource,
     ListSourcesSourcesListAwsRedshiftSourceConfig,
@@ -1408,14 +1536,19 @@
     ListSourcesSourcesListGcpPubSubSourceWindows,
     ListSourcesSourcesListGcpStorageSource,
     ListSourcesSourcesListGcpStorageSourceConfig,
     ListSourcesSourcesListGcpStorageSourceConfigCsv,
     ListSourcesSourcesListGcpStorageSourceCredential,
     ListSourcesSourcesListGcpStorageSourceSegmentations,
     ListSourcesSourcesListGcpStorageSourceWindows,
+    ListSourcesSourcesListKafkaSource,
+    ListSourcesSourcesListKafkaSourceConfig,
+    ListSourcesSourcesListKafkaSourceCredential,
+    ListSourcesSourcesListKafkaSourceSegmentations,
+    ListSourcesSourcesListKafkaSourceWindows,
     ListSourcesSourcesListPostgreSqlSource,
     ListSourcesSourcesListPostgreSqlSourceConfig,
     ListSourcesSourcesListPostgreSqlSourceCredential,
     ListSourcesSourcesListPostgreSqlSourceSegmentations,
     ListSourcesSourcesListPostgreSqlSourceWindows,
     ListSourcesSourcesListSnowflakeSource,
     ListSourcesSourcesListSnowflakeSourceConfig,
@@ -1550,14 +1683,22 @@
 )
 from .start_source import (
     StartSource,
     StartSourceSourceStart,
     StartSourceSourceStartErrors,
 )
 from .stop_source import StopSource, StopSourceSourceStop, StopSourceSourceStopErrors
+from .update_aws_athena_credential import (
+    UpdateAwsAthenaCredential,
+    UpdateAwsAthenaCredentialAwsAthenaCredentialUpdate,
+)
+from .update_aws_athena_source import (
+    UpdateAwsAthenaSource,
+    UpdateAwsAthenaSourceAwsAthenaSourceUpdate,
+)
 from .update_aws_credential import (
     UpdateAwsCredential,
     UpdateAwsCredentialAwsCredentialUpdate,
 )
 from .update_aws_kinesis_destination import (
     UpdateAwsKinesisDestination,
     UpdateAwsKinesisDestinationAwsKinesisDestinationUpdate,
@@ -1575,14 +1716,26 @@
     UpdateAwsRedshiftSourceAwsRedshiftSourceUpdate,
 )
 from .update_aws_s3_source import UpdateAwsS3Source, UpdateAwsS3SourceAwsS3SourceUpdate
 from .update_categorical_distribution_validator import (
     UpdateCategoricalDistributionValidator,
     UpdateCategoricalDistributionValidatorCategoricalDistributionValidatorUpdate,
 )
+from .update_channel_namespace import (
+    UpdateChannelNamespace,
+    UpdateChannelNamespaceChannelNamespaceUpdate,
+)
+from .update_credential_namespace import (
+    UpdateCredentialNamespace,
+    UpdateCredentialNamespaceCredentialNamespaceUpdate,
+)
+from .update_destination_namespace import (
+    UpdateDestinationNamespace,
+    UpdateDestinationNamespaceDestinationNamespaceUpdate,
+)
 from .update_fixed_batch_window import (
     UpdateFixedBatchWindow,
     UpdateFixedBatchWindowFixedBatchWindowUpdate,
 )
 from .update_freshness_validator import (
     UpdateFreshnessValidator,
     UpdateFreshnessValidatorFreshnessValidatorUpdate,
@@ -1607,22 +1760,39 @@
     UpdateGcpPubSubSource,
     UpdateGcpPubSubSourceGcpPubSubSourceUpdate,
 )
 from .update_gcp_storage_source import (
     UpdateGcpStorageSource,
     UpdateGcpStorageSourceGcpStorageSourceUpdate,
 )
+from .update_identity_provider_namespace import (
+    UpdateIdentityProviderNamespace,
+    UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate,
+)
+from .update_kafka_sasl_plain_credential import (
+    UpdateKafkaSaslPlainCredential,
+    UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate,
+)
+from .update_kafka_source import UpdateKafkaSource, UpdateKafkaSourceKafkaSourceUpdate
+from .update_kafka_ssl_credential import (
+    UpdateKafkaSslCredential,
+    UpdateKafkaSslCredentialKafkaSslCredentialUpdate,
+)
 from .update_local_identity_provider import (
     UpdateLocalIdentityProvider,
     UpdateLocalIdentityProviderLocalIdentityProviderUpdate,
 )
 from .update_notification_rule import (
     UpdateNotificationRule,
     UpdateNotificationRuleNotificationRuleUpdate,
 )
+from .update_notification_rule_namespace import (
+    UpdateNotificationRuleNamespace,
+    UpdateNotificationRuleNamespaceNotificationRuleNamespaceUpdate,
+)
 from .update_numeric_anomaly_validator import (
     UpdateNumericAnomalyValidator,
     UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate,
 )
 from .update_numeric_distribution_validator import (
     UpdateNumericDistributionValidator,
     UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate,
@@ -1647,14 +1817,18 @@
     UpdateRelativeVolumeValidator,
     UpdateRelativeVolumeValidatorRelativeVolumeValidatorUpdate,
 )
 from .update_saml_identity_provider import (
     UpdateSamlIdentityProvider,
     UpdateSamlIdentityProviderSamlIdentityProviderUpdate,
 )
+from .update_segmentation_namespace import (
+    UpdateSegmentationNamespace,
+    UpdateSegmentationNamespaceSegmentationNamespaceUpdate,
+)
 from .update_sessionized_window import (
     UpdateSessionizedWindow,
     UpdateSessionizedWindowSessionizedWindowUpdate,
 )
 from .update_slack_channel import (
     UpdateSlackChannel,
     UpdateSlackChannelSlackChannelUpdate,
@@ -1667,19 +1841,31 @@
     UpdateSnowflakeDestination,
     UpdateSnowflakeDestinationSnowflakeDestinationUpdate,
 )
 from .update_snowflake_source import (
     UpdateSnowflakeSource,
     UpdateSnowflakeSourceSnowflakeSourceUpdate,
 )
+from .update_source_namespace import (
+    UpdateSourceNamespace,
+    UpdateSourceNamespaceSourceNamespaceUpdate,
+)
 from .update_tumbling_window import (
     UpdateTumblingWindow,
     UpdateTumblingWindowTumblingWindowUpdate,
 )
 from .update_user import UpdateUser, UpdateUserUserUpdate
+from .update_user_namespace import (
+    UpdateUserNamespace,
+    UpdateUserNamespaceUserNamespaceUpdate,
+)
+from .update_validator_namespace import (
+    UpdateValidatorNamespace,
+    UpdateValidatorNamespaceValidatorNamespaceUpdate,
+)
 from .update_validator_with_dynamic_threshold import (
     UpdateValidatorWithDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateErrors,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidator,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfig,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold,
@@ -1968,20 +2154,29 @@
     UpdateVolumeValidator,
     UpdateVolumeValidatorVolumeValidatorUpdate,
 )
 from .update_webhook_channel import (
     UpdateWebhookChannel,
     UpdateWebhookChannelWebhookChannelUpdate,
 )
+from .update_window_namespace import (
+    UpdateWindowNamespace,
+    UpdateWindowNamespaceWindowNamespaceUpdate,
+)
 
 __all__ = [
     "ApiErrorCode",
     "ApplyValidatorRecommendation",
     "ApplyValidatorRecommendationValidatorRecommendationApply",
     "AsyncBaseClient",
+    "AwsAthenaCredentialCreateInput",
+    "AwsAthenaCredentialUpdateInput",
+    "AwsAthenaInferSchemaInput",
+    "AwsAthenaSourceCreateInput",
+    "AwsAthenaSourceUpdateInput",
     "AwsCredentialCreateInput",
     "AwsCredentialSecretChanged",
     "AwsCredentialSecretChangedAwsCredentialSecretChanged",
     "AwsCredentialSecretChangedInput",
     "AwsCredentialUpdateInput",
     "AwsKinesisDestinationCreateInput",
     "AwsKinesisDestinationUpdateInput",
@@ -2022,14 +2217,18 @@
     "ChannelUpdateChannelSlackChannel",
     "ChannelUpdateChannelSlackChannelConfig",
     "ChannelUpdateChannelWebhookChannel",
     "ChannelUpdateChannelWebhookChannelConfig",
     "ChannelUpdateErrors",
     "Client",
     "ComparisonOperator",
+    "CreateAwsAthenaCredential",
+    "CreateAwsAthenaCredentialAwsAthenaCredentialCreate",
+    "CreateAwsAthenaSource",
+    "CreateAwsAthenaSourceAwsAthenaSourceCreate",
     "CreateAwsCredential",
     "CreateAwsCredentialAwsCredentialCreate",
     "CreateAwsKinesisDestination",
     "CreateAwsKinesisDestinationAwsKinesisDestinationCreate",
     "CreateAwsKinesisSource",
     "CreateAwsKinesisSourceAwsKinesisSourceCreate",
     "CreateAwsRedshiftCredential",
@@ -2062,14 +2261,20 @@
     "CreateGcpCredentialGcpCredentialCreate",
     "CreateGcpPubSubLiteSource",
     "CreateGcpPubSubLiteSourceGcpPubSubLiteSourceCreate",
     "CreateGcpPubSubSource",
     "CreateGcpPubSubSourceGcpPubSubSourceCreate",
     "CreateGcpStorageSource",
     "CreateGcpStorageSourceGcpStorageSourceCreate",
+    "CreateKafkaSaslPlainCredential",
+    "CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate",
+    "CreateKafkaSource",
+    "CreateKafkaSourceKafkaSourceCreate",
+    "CreateKafkaSslCredential",
+    "CreateKafkaSslCredentialKafkaSslCredentialCreate",
     "CreateNotificationRule",
     "CreateNotificationRuleNotificationRuleCreate",
     "CreateNumericAnomalyValidatorWithDynamicThreshold",
     "CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate",
     "CreateNumericAnomalyValidatorWithFixedThreshold",
     "CreateNumericAnomalyValidatorWithFixedThresholdNumericAnomalyValidatorWithFixedThresholdCreate",
     "CreateNumericDistributionValidatorWithDynamicThreshold",
@@ -2119,32 +2324,44 @@
     "CreateVolumeValidatorWithDynamicThreshold",
     "CreateVolumeValidatorWithDynamicThresholdVolumeValidatorWithDynamicThresholdCreate",
     "CreateVolumeValidatorWithFixedThreshold",
     "CreateVolumeValidatorWithFixedThresholdVolumeValidatorWithFixedThresholdCreate",
     "CreateWebhookChannel",
     "CreateWebhookChannelWebhookChannelCreate",
     "CredentialCreation",
+    "CredentialCreationCredentialAwsAthenaCredential",
+    "CredentialCreationCredentialAwsAthenaCredentialConfig",
     "CredentialCreationCredentialAwsCredential",
     "CredentialCreationCredentialAwsCredentialConfig",
     "CredentialCreationCredentialAwsRedshiftCredential",
     "CredentialCreationCredentialAwsRedshiftCredentialConfig",
     "CredentialCreationCredentialCredential",
+    "CredentialCreationCredentialKafkaSASLPlainCredential",
+    "CredentialCreationCredentialKafkaSASLPlainCredentialConfig",
+    "CredentialCreationCredentialKafkaSSLCredential",
+    "CredentialCreationCredentialKafkaSSLCredentialConfig",
     "CredentialCreationCredentialPostgreSqlCredential",
     "CredentialCreationCredentialPostgreSqlCredentialConfig",
     "CredentialCreationCredentialSnowflakeCredential",
     "CredentialCreationCredentialSnowflakeCredentialConfig",
     "CredentialCreationErrors",
     "CredentialSecretChanged",
     "CredentialSecretChangedErrors",
     "CredentialUpdate",
+    "CredentialUpdateCredentialAwsAthenaCredential",
+    "CredentialUpdateCredentialAwsAthenaCredentialConfig",
     "CredentialUpdateCredentialAwsCredential",
     "CredentialUpdateCredentialAwsCredentialConfig",
     "CredentialUpdateCredentialAwsRedshiftCredential",
     "CredentialUpdateCredentialAwsRedshiftCredentialConfig",
     "CredentialUpdateCredentialCredential",
+    "CredentialUpdateCredentialKafkaSASLPlainCredential",
+    "CredentialUpdateCredentialKafkaSASLPlainCredentialConfig",
+    "CredentialUpdateCredentialKafkaSSLCredential",
+    "CredentialUpdateCredentialKafkaSSLCredentialConfig",
     "CredentialUpdateCredentialPostgreSqlCredential",
     "CredentialUpdateCredentialPostgreSqlCredentialConfig",
     "CredentialUpdateCredentialSnowflakeCredential",
     "CredentialUpdateCredentialSnowflakeCredentialConfig",
     "CredentialUpdateErrors",
     "CsvParserInput",
     "DecisionBoundsType",
@@ -2255,19 +2472,25 @@
     "GetChannels",
     "GetChannelsChannelsChannel",
     "GetChannelsChannelsSlackChannel",
     "GetChannelsChannelsSlackChannelConfig",
     "GetChannelsChannelsWebhookChannel",
     "GetChannelsChannelsWebhookChannelConfig",
     "GetCredentialByResourceName",
+    "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential",
+    "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameAwsCredential",
     "GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential",
     "GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameCredential",
+    "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential",
+    "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig",
+    "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential",
+    "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential",
     "GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredentialConfig",
     "GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential",
     "GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig",
     "GetDestinationByResourceName",
     "GetDestinationByResourceNameDestinationByResourceNameAwsKinesisDestination",
     "GetDestinationByResourceNameDestinationByResourceNameAwsKinesisDestinationConfig",
@@ -2299,22 +2522,32 @@
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithFixedThreshold",
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationMetricValidatorMetricWithMonotonicThreshold",
     "GetIncidentsIncidentsValidatorThresholdFailureNotificationSegment",
     "GetNotificationRuleByResourceName",
     "GetNotificationRuleByResourceNameNotificationRuleByResourceName",
     "GetNotificationRules",
     "GetNotificationRulesNotificationRules",
+    "GetRecommendation",
+    "GetRecommendationRecommendationRecommendation",
+    "GetRecommendationRecommendationValidatorCreateRecommendation",
+    "GetRecommendationRecommendationValidatorDeleteRecommendation",
+    "GetRecommendationRecommendationValidatorUpdateRecommendation",
     "GetSegmentIncidents",
     "GetSegmentIncidentsSegmentIncidents",
     "GetSegmentation",
     "GetSegmentationByResourceName",
     "GetSegmentationByResourceNameSegmentationByResourceName",
     "GetSegmentationSegmentation",
     "GetSource",
     "GetSourceByResourceName",
+    "GetSourceByResourceNameSourceByResourceNameAwsAthenaSource",
+    "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceConfig",
+    "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceCredential",
+    "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceSegmentations",
+    "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceWindows",
     "GetSourceByResourceNameSourceByResourceNameAwsKinesisSource",
     "GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceConfig",
     "GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceCredential",
     "GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceSegmentations",
     "GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceWindows",
     "GetSourceByResourceNameSourceByResourceNameAwsRedshiftSource",
     "GetSourceByResourceNameSourceByResourceNameAwsRedshiftSourceConfig",
@@ -2344,14 +2577,19 @@
     "GetSourceByResourceNameSourceByResourceNameGcpPubSubSourceWindows",
     "GetSourceByResourceNameSourceByResourceNameGcpStorageSource",
     "GetSourceByResourceNameSourceByResourceNameGcpStorageSourceConfig",
     "GetSourceByResourceNameSourceByResourceNameGcpStorageSourceConfigCsv",
     "GetSourceByResourceNameSourceByResourceNameGcpStorageSourceCredential",
     "GetSourceByResourceNameSourceByResourceNameGcpStorageSourceSegmentations",
     "GetSourceByResourceNameSourceByResourceNameGcpStorageSourceWindows",
+    "GetSourceByResourceNameSourceByResourceNameKafkaSource",
+    "GetSourceByResourceNameSourceByResourceNameKafkaSourceConfig",
+    "GetSourceByResourceNameSourceByResourceNameKafkaSourceCredential",
+    "GetSourceByResourceNameSourceByResourceNameKafkaSourceSegmentations",
+    "GetSourceByResourceNameSourceByResourceNameKafkaSourceWindows",
     "GetSourceByResourceNameSourceByResourceNamePostgreSqlSource",
     "GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceConfig",
     "GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceCredential",
     "GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceSegmentations",
     "GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceWindows",
     "GetSourceByResourceNameSourceByResourceNameSnowflakeSource",
     "GetSourceByResourceNameSourceByResourceNameSnowflakeSourceConfig",
@@ -2370,55 +2608,68 @@
     "GetSourceRecommendedValidatorsSource",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorStats",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidator",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorProgress",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfig",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSegmentation",
     "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSource",
+    "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorStats",
+    "GetSourceSourceAwsAthenaSource",
+    "GetSourceSourceAwsAthenaSourceConfig",
+    "GetSourceSourceAwsAthenaSourceCredential",
+    "GetSourceSourceAwsAthenaSourceSegmentations",
+    "GetSourceSourceAwsAthenaSourceWindows",
     "GetSourceSourceAwsKinesisSource",
     "GetSourceSourceAwsKinesisSourceConfig",
     "GetSourceSourceAwsKinesisSourceCredential",
     "GetSourceSourceAwsKinesisSourceSegmentations",
     "GetSourceSourceAwsKinesisSourceWindows",
     "GetSourceSourceAwsRedshiftSource",
     "GetSourceSourceAwsRedshiftSourceConfig",
@@ -2448,14 +2699,19 @@
     "GetSourceSourceGcpPubSubSourceWindows",
     "GetSourceSourceGcpStorageSource",
     "GetSourceSourceGcpStorageSourceConfig",
     "GetSourceSourceGcpStorageSourceConfigCsv",
     "GetSourceSourceGcpStorageSourceCredential",
     "GetSourceSourceGcpStorageSourceSegmentations",
     "GetSourceSourceGcpStorageSourceWindows",
+    "GetSourceSourceKafkaSource",
+    "GetSourceSourceKafkaSourceConfig",
+    "GetSourceSourceKafkaSourceCredential",
+    "GetSourceSourceKafkaSourceSegmentations",
+    "GetSourceSourceKafkaSourceWindows",
     "GetSourceSourcePostgreSqlSource",
     "GetSourceSourcePostgreSqlSourceConfig",
     "GetSourceSourcePostgreSqlSourceCredential",
     "GetSourceSourcePostgreSqlSourceSegmentations",
     "GetSourceSourcePostgreSqlSourceWindows",
     "GetSourceSourceSnowflakeSource",
     "GetSourceSourceSnowflakeSourceConfig",
@@ -2699,30 +2955,51 @@
     "IdentityProviderUpdate",
     "IdentityProviderUpdateErrorCode",
     "IdentityProviderUpdateErrors",
     "IdentityProviderUpdateIdentityProviderIdentityProvider",
     "IdentityProviderUpdateIdentityProviderSamlIdentityProvider",
     "IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig",
     "IncidentsInput",
+    "InferAwsAthenaSchema",
     "InferAwsKinesisSchema",
     "InferAwsRedshiftSchema",
     "InferAwsS3Schema",
     "InferDemoSchema",
     "InferGcpBigQuerySchema",
     "InferGcpPubSubLiteSchema",
     "InferGcpPubSubSchema",
     "InferGcpStorageSchema",
+    "InferKafkaSchema",
     "InferPostgreSqlSchema",
     "InferSnowflakeSchema",
+    "KafkaInferSchemaInput",
+    "KafkaSASLPlainCredentialCreateInput",
+    "KafkaSASLPlainCredentialSecretChangedInput",
+    "KafkaSASLPlainCredentialUpdateInput",
+    "KafkaSSLCredentialCreateInput",
+    "KafkaSSLCredentialSecretChangedInput",
+    "KafkaSSLCredentialUpdateInput",
+    "KafkaSaslPlainCredentialSecretChanged",
+    "KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged",
+    "KafkaSourceCreateInput",
+    "KafkaSourceUpdateInput",
+    "KafkaSslCredentialSecretChanged",
+    "KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged",
     "ListCredentials",
+    "ListCredentialsCredentialsListAwsAthenaCredential",
+    "ListCredentialsCredentialsListAwsAthenaCredentialConfig",
     "ListCredentialsCredentialsListAwsCredential",
     "ListCredentialsCredentialsListAwsCredentialConfig",
     "ListCredentialsCredentialsListAwsRedshiftCredential",
     "ListCredentialsCredentialsListAwsRedshiftCredentialConfig",
     "ListCredentialsCredentialsListCredential",
+    "ListCredentialsCredentialsListKafkaSASLPlainCredential",
+    "ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig",
+    "ListCredentialsCredentialsListKafkaSSLCredential",
+    "ListCredentialsCredentialsListKafkaSSLCredentialConfig",
     "ListCredentialsCredentialsListPostgreSqlCredential",
     "ListCredentialsCredentialsListPostgreSqlCredentialConfig",
     "ListCredentialsCredentialsListSnowflakeCredential",
     "ListCredentialsCredentialsListSnowflakeCredentialConfig",
     "ListDestinations",
     "ListDestinationsDestinationsListAwsKinesisDestination",
     "ListDestinationsDestinationsListAwsKinesisDestinationConfig",
@@ -2734,14 +3011,19 @@
     "ListDestinationsDestinationsListGcpBigQueryDestinationCredential",
     "ListDestinationsDestinationsListSnowflakeDestination",
     "ListDestinationsDestinationsListSnowflakeDestinationConfig",
     "ListDestinationsDestinationsListSnowflakeDestinationCredential",
     "ListSegmentations",
     "ListSegmentationsSegmentationsList",
     "ListSources",
+    "ListSourcesSourcesListAwsAthenaSource",
+    "ListSourcesSourcesListAwsAthenaSourceConfig",
+    "ListSourcesSourcesListAwsAthenaSourceCredential",
+    "ListSourcesSourcesListAwsAthenaSourceSegmentations",
+    "ListSourcesSourcesListAwsAthenaSourceWindows",
     "ListSourcesSourcesListAwsKinesisSource",
     "ListSourcesSourcesListAwsKinesisSourceConfig",
     "ListSourcesSourcesListAwsKinesisSourceCredential",
     "ListSourcesSourcesListAwsKinesisSourceSegmentations",
     "ListSourcesSourcesListAwsKinesisSourceWindows",
     "ListSourcesSourcesListAwsRedshiftSource",
     "ListSourcesSourcesListAwsRedshiftSourceConfig",
@@ -2771,14 +3053,19 @@
     "ListSourcesSourcesListGcpPubSubSourceWindows",
     "ListSourcesSourcesListGcpStorageSource",
     "ListSourcesSourcesListGcpStorageSourceConfig",
     "ListSourcesSourcesListGcpStorageSourceConfigCsv",
     "ListSourcesSourcesListGcpStorageSourceCredential",
     "ListSourcesSourcesListGcpStorageSourceSegmentations",
     "ListSourcesSourcesListGcpStorageSourceWindows",
+    "ListSourcesSourcesListKafkaSource",
+    "ListSourcesSourcesListKafkaSourceConfig",
+    "ListSourcesSourcesListKafkaSourceCredential",
+    "ListSourcesSourcesListKafkaSourceSegmentations",
+    "ListSourcesSourcesListKafkaSourceWindows",
     "ListSourcesSourcesListPostgreSqlSource",
     "ListSourcesSourcesListPostgreSqlSourceConfig",
     "ListSourcesSourcesListPostgreSqlSourceCredential",
     "ListSourcesSourcesListPostgreSqlSourceSegmentations",
     "ListSourcesSourcesListPostgreSqlSourceWindows",
     "ListSourcesSourcesListSnowflakeSource",
     "ListSourcesSourcesListSnowflakeSourceConfig",
@@ -2891,14 +3178,16 @@
     "ListWindowsWindowsListTumblingWindow",
     "ListWindowsWindowsListTumblingWindowConfig",
     "ListWindowsWindowsListTumblingWindowSource",
     "ListWindowsWindowsListWindow",
     "ListWindowsWindowsListWindowSource",
     "LocalIdentityProviderUpdateInput",
     "MonotonicThresholdCreateInput",
+    "NamespaceUpdate",
+    "NamespaceUpdateErrors",
     "NotificationRuleCreateInput",
     "NotificationRuleCreation",
     "NotificationRuleCreationErrors",
     "NotificationRuleCreationNotificationRule",
     "NotificationRuleDeleteInput",
     "NotificationRuleDeletion",
     "NotificationRuleDeletionErrors",
@@ -2940,14 +3229,15 @@
     "RelativeTimeMetric",
     "RelativeTimeValidatorCreateInput",
     "RelativeTimeValidatorUpdateInput",
     "RelativeVolumeMetric",
     "RelativeVolumeValidatorCreateInput",
     "RelativeVolumeValidatorUpdateInput",
     "ResourceFilter",
+    "ResourceNamespaceUpdateInput",
     "Role",
     "SamlIdentityProviderCreateInput",
     "SamlIdentityProviderUpdateInput",
     "SegmentDetails",
     "SegmentDetailsFields",
     "SegmentIncidentsInput",
     "SegmentationCreateInput",
@@ -2975,14 +3265,19 @@
     "SnowflakeInferSchemaInput",
     "SnowflakeSourceCreateInput",
     "SnowflakeSourceUpdateInput",
     "SourceConfigCreateInput",
     "SourceConfigUpdateInput",
     "SourceCreation",
     "SourceCreationErrors",
+    "SourceCreationSourceAwsAthenaSource",
+    "SourceCreationSourceAwsAthenaSourceConfig",
+    "SourceCreationSourceAwsAthenaSourceCredential",
+    "SourceCreationSourceAwsAthenaSourceSegmentations",
+    "SourceCreationSourceAwsAthenaSourceWindows",
     "SourceCreationSourceAwsKinesisSource",
     "SourceCreationSourceAwsKinesisSourceConfig",
     "SourceCreationSourceAwsKinesisSourceCredential",
     "SourceCreationSourceAwsKinesisSourceSegmentations",
     "SourceCreationSourceAwsKinesisSourceWindows",
     "SourceCreationSourceAwsRedshiftSource",
     "SourceCreationSourceAwsRedshiftSourceConfig",
@@ -3012,14 +3307,19 @@
     "SourceCreationSourceGcpPubSubSourceWindows",
     "SourceCreationSourceGcpStorageSource",
     "SourceCreationSourceGcpStorageSourceConfig",
     "SourceCreationSourceGcpStorageSourceConfigCsv",
     "SourceCreationSourceGcpStorageSourceCredential",
     "SourceCreationSourceGcpStorageSourceSegmentations",
     "SourceCreationSourceGcpStorageSourceWindows",
+    "SourceCreationSourceKafkaSource",
+    "SourceCreationSourceKafkaSourceConfig",
+    "SourceCreationSourceKafkaSourceCredential",
+    "SourceCreationSourceKafkaSourceSegmentations",
+    "SourceCreationSourceKafkaSourceWindows",
     "SourceCreationSourcePostgreSqlSource",
     "SourceCreationSourcePostgreSqlSourceConfig",
     "SourceCreationSourcePostgreSqlSourceCredential",
     "SourceCreationSourcePostgreSqlSourceSegmentations",
     "SourceCreationSourcePostgreSqlSourceWindows",
     "SourceCreationSourceSnowflakeSource",
     "SourceCreationSourceSnowflakeSourceConfig",
@@ -3030,14 +3330,19 @@
     "SourceCreationSourceSourceCredential",
     "SourceCreationSourceSourceSegmentations",
     "SourceCreationSourceSourceWindows",
     "SourceIncidentsInput",
     "SourceState",
     "SourceUpdate",
     "SourceUpdateErrors",
+    "SourceUpdateSourceAwsAthenaSource",
+    "SourceUpdateSourceAwsAthenaSourceConfig",
+    "SourceUpdateSourceAwsAthenaSourceCredential",
+    "SourceUpdateSourceAwsAthenaSourceSegmentations",
+    "SourceUpdateSourceAwsAthenaSourceWindows",
     "SourceUpdateSourceAwsKinesisSource",
     "SourceUpdateSourceAwsKinesisSourceConfig",
     "SourceUpdateSourceAwsKinesisSourceCredential",
     "SourceUpdateSourceAwsKinesisSourceSegmentations",
     "SourceUpdateSourceAwsKinesisSourceWindows",
     "SourceUpdateSourceAwsRedshiftSource",
     "SourceUpdateSourceAwsRedshiftSourceConfig",
@@ -3067,14 +3372,19 @@
     "SourceUpdateSourceGcpPubSubSourceWindows",
     "SourceUpdateSourceGcpStorageSource",
     "SourceUpdateSourceGcpStorageSourceConfig",
     "SourceUpdateSourceGcpStorageSourceConfigCsv",
     "SourceUpdateSourceGcpStorageSourceCredential",
     "SourceUpdateSourceGcpStorageSourceSegmentations",
     "SourceUpdateSourceGcpStorageSourceWindows",
+    "SourceUpdateSourceKafkaSource",
+    "SourceUpdateSourceKafkaSourceConfig",
+    "SourceUpdateSourceKafkaSourceCredential",
+    "SourceUpdateSourceKafkaSourceSegmentations",
+    "SourceUpdateSourceKafkaSourceWindows",
     "SourceUpdateSourcePostgreSqlSource",
     "SourceUpdateSourcePostgreSqlSourceConfig",
     "SourceUpdateSourcePostgreSqlSourceCredential",
     "SourceUpdateSourcePostgreSqlSourceSegmentations",
     "SourceUpdateSourcePostgreSqlSourceWindows",
     "SourceUpdateSourceSnowflakeSource",
     "SourceUpdateSourceSnowflakeSourceConfig",
@@ -3090,28 +3400,38 @@
     "StartSourceSourceStartErrors",
     "StopSource",
     "StopSourceSourceStop",
     "StopSourceSourceStopErrors",
     "TimeRangeInput",
     "TumblingWindowCreateInput",
     "TumblingWindowUpdateInput",
+    "UpdateAwsAthenaCredential",
+    "UpdateAwsAthenaCredentialAwsAthenaCredentialUpdate",
+    "UpdateAwsAthenaSource",
+    "UpdateAwsAthenaSourceAwsAthenaSourceUpdate",
     "UpdateAwsCredential",
     "UpdateAwsCredentialAwsCredentialUpdate",
     "UpdateAwsKinesisDestination",
     "UpdateAwsKinesisDestinationAwsKinesisDestinationUpdate",
     "UpdateAwsKinesisSource",
     "UpdateAwsKinesisSourceAwsKinesisSourceUpdate",
     "UpdateAwsRedshiftCredential",
     "UpdateAwsRedshiftCredentialAwsRedshiftCredentialUpdate",
     "UpdateAwsRedshiftSource",
     "UpdateAwsRedshiftSourceAwsRedshiftSourceUpdate",
     "UpdateAwsS3Source",
     "UpdateAwsS3SourceAwsS3SourceUpdate",
     "UpdateCategoricalDistributionValidator",
     "UpdateCategoricalDistributionValidatorCategoricalDistributionValidatorUpdate",
+    "UpdateChannelNamespace",
+    "UpdateChannelNamespaceChannelNamespaceUpdate",
+    "UpdateCredentialNamespace",
+    "UpdateCredentialNamespaceCredentialNamespaceUpdate",
+    "UpdateDestinationNamespace",
+    "UpdateDestinationNamespaceDestinationNamespaceUpdate",
     "UpdateFixedBatchWindow",
     "UpdateFixedBatchWindowFixedBatchWindowUpdate",
     "UpdateFreshnessValidator",
     "UpdateFreshnessValidatorFreshnessValidatorUpdate",
     "UpdateGcpBigQueryDestination",
     "UpdateGcpBigQueryDestinationGcpBigQueryDestinationUpdate",
     "UpdateGcpBigQuerySource",
@@ -3120,17 +3440,27 @@
     "UpdateGcpCredentialGcpCredentialUpdate",
     "UpdateGcpPubSubLiteSource",
     "UpdateGcpPubSubLiteSourceGcpPubSubLiteSourceUpdate",
     "UpdateGcpPubSubSource",
     "UpdateGcpPubSubSourceGcpPubSubSourceUpdate",
     "UpdateGcpStorageSource",
     "UpdateGcpStorageSourceGcpStorageSourceUpdate",
+    "UpdateIdentityProviderNamespace",
+    "UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate",
+    "UpdateKafkaSaslPlainCredential",
+    "UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate",
+    "UpdateKafkaSource",
+    "UpdateKafkaSourceKafkaSourceUpdate",
+    "UpdateKafkaSslCredential",
+    "UpdateKafkaSslCredentialKafkaSslCredentialUpdate",
     "UpdateLocalIdentityProvider",
     "UpdateLocalIdentityProviderLocalIdentityProviderUpdate",
     "UpdateNotificationRule",
+    "UpdateNotificationRuleNamespace",
+    "UpdateNotificationRuleNamespaceNotificationRuleNamespaceUpdate",
     "UpdateNotificationRuleNotificationRuleUpdate",
     "UpdateNumericAnomalyValidator",
     "UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate",
     "UpdateNumericDistributionValidator",
     "UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate",
     "UpdateNumericValidator",
     "UpdateNumericValidatorNumericValidatorUpdate",
@@ -3140,28 +3470,36 @@
     "UpdatePostgreSqlSourcePostgreSqlSourceUpdate",
     "UpdateRelativeTimeValidator",
     "UpdateRelativeTimeValidatorRelativeTimeValidatorUpdate",
     "UpdateRelativeVolumeValidator",
     "UpdateRelativeVolumeValidatorRelativeVolumeValidatorUpdate",
     "UpdateSamlIdentityProvider",
     "UpdateSamlIdentityProviderSamlIdentityProviderUpdate",
+    "UpdateSegmentationNamespace",
+    "UpdateSegmentationNamespaceSegmentationNamespaceUpdate",
     "UpdateSessionizedWindow",
     "UpdateSessionizedWindowSessionizedWindowUpdate",
     "UpdateSlackChannel",
     "UpdateSlackChannelSlackChannelUpdate",
     "UpdateSnowflakeCredential",
     "UpdateSnowflakeCredentialSnowflakeCredentialUpdate",
     "UpdateSnowflakeDestination",
     "UpdateSnowflakeDestinationSnowflakeDestinationUpdate",
     "UpdateSnowflakeSource",
     "UpdateSnowflakeSourceSnowflakeSourceUpdate",
+    "UpdateSourceNamespace",
+    "UpdateSourceNamespaceSourceNamespaceUpdate",
     "UpdateTumblingWindow",
     "UpdateTumblingWindowTumblingWindowUpdate",
     "UpdateUser",
+    "UpdateUserNamespace",
+    "UpdateUserNamespaceUserNamespaceUpdate",
     "UpdateUserUserUpdate",
+    "UpdateValidatorNamespace",
+    "UpdateValidatorNamespaceValidatorNamespaceUpdate",
     "UpdateValidatorWithDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateErrors",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidator",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfig",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdDynamicThreshold",
     "UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdateValidatorCategoricalDistributionValidatorConfigThresholdFixedThreshold",
@@ -3440,14 +3778,16 @@
     "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigSegmentation",
     "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigSource",
     "UpdateValidatorWithMonotonicThresholdValidatorWithMonotonicThresholdUpdateValidatorVolumeValidatorSourceConfigWindow",
     "UpdateVolumeValidator",
     "UpdateVolumeValidatorVolumeValidatorUpdate",
     "UpdateWebhookChannel",
     "UpdateWebhookChannelWebhookChannelUpdate",
+    "UpdateWindowNamespace",
+    "UpdateWindowNamespaceWindowNamespaceUpdate",
     "UserCreateInput",
     "UserCreation",
     "UserCreationErrors",
     "UserCreationUser",
     "UserDeleteErrorCode",
     "UserDeleteInput",
     "UserDeletion",
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/apply_validator_recommendation.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/apply_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/async_base_client.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/aws_credential_secret_changed.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/aws_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/aws_redshift_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/backfill_source.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/backfill_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/base_model.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/client.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union
+from typing import Any, List, Optional, Union
 
 from validio_sdk.scalars import (
     CredentialId,
     DestinationId,
     JsonTypeDefinition,
     SegmentationId,
     SourceId,
@@ -21,14 +21,22 @@
 )
 from .aws_redshift_credential_secret_changed import (
     AwsRedshiftCredentialSecretChanged,
     AwsRedshiftCredentialSecretChangedAwsRedshiftCredentialSecretChanged,
 )
 from .backfill_source import BackfillSource, BackfillSourceSourceBackfill
 from .base_model import UNSET, UnsetType
+from .create_aws_athena_credential import (
+    CreateAwsAthenaCredential,
+    CreateAwsAthenaCredentialAwsAthenaCredentialCreate,
+)
+from .create_aws_athena_source import (
+    CreateAwsAthenaSource,
+    CreateAwsAthenaSourceAwsAthenaSourceCreate,
+)
 from .create_aws_credential import (
     CreateAwsCredential,
     CreateAwsCredentialAwsCredentialCreate,
 )
 from .create_aws_kinesis_destination import (
     CreateAwsKinesisDestination,
     CreateAwsKinesisDestinationAwsKinesisDestinationCreate,
@@ -92,14 +100,23 @@
     CreateGcpPubSubSource,
     CreateGcpPubSubSourceGcpPubSubSourceCreate,
 )
 from .create_gcp_storage_source import (
     CreateGcpStorageSource,
     CreateGcpStorageSourceGcpStorageSourceCreate,
 )
+from .create_kafka_sasl_plain_credential import (
+    CreateKafkaSaslPlainCredential,
+    CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate,
+)
+from .create_kafka_source import CreateKafkaSource, CreateKafkaSourceKafkaSourceCreate
+from .create_kafka_ssl_credential import (
+    CreateKafkaSslCredential,
+    CreateKafkaSslCredentialKafkaSslCredentialCreate,
+)
 from .create_notification_rule import (
     CreateNotificationRule,
     CreateNotificationRuleNotificationRuleCreate,
 )
 from .create_numeric_anomaly_validator_with_dynamic_threshold import (
     CreateNumericAnomalyValidatorWithDynamicThreshold,
     CreateNumericAnomalyValidatorWithDynamicThresholdNumericAnomalyValidatorWithDynamicThresholdCreate,
@@ -250,17 +267,20 @@
     GetChannels,
     GetChannelsChannelsChannel,
     GetChannelsChannelsSlackChannel,
     GetChannelsChannelsWebhookChannel,
 )
 from .get_credential_by_resource_name import (
     GetCredentialByResourceName,
+    GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsCredential,
     GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential,
     GetCredentialByResourceNameCredentialByResourceNameCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential,
+    GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential,
     GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential,
     GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential,
 )
 from .get_destination_by_resource_name import (
     GetDestinationByResourceName,
     GetDestinationByResourceNameDestinationByResourceNameAwsKinesisDestination,
     GetDestinationByResourceNameDestinationByResourceNameDestination,
@@ -288,45 +308,56 @@
     GetNotificationRuleByResourceName,
     GetNotificationRuleByResourceNameNotificationRuleByResourceName,
 )
 from .get_notification_rules import (
     GetNotificationRules,
     GetNotificationRulesNotificationRules,
 )
+from .get_recommendation import (
+    GetRecommendation,
+    GetRecommendationRecommendationRecommendation,
+    GetRecommendationRecommendationValidatorCreateRecommendation,
+    GetRecommendationRecommendationValidatorDeleteRecommendation,
+    GetRecommendationRecommendationValidatorUpdateRecommendation,
+)
 from .get_segment_incidents import (
     GetSegmentIncidents,
     GetSegmentIncidentsSegmentIncidents,
 )
 from .get_segmentation import GetSegmentation, GetSegmentationSegmentation
 from .get_segmentation_by_resource_name import (
     GetSegmentationByResourceName,
     GetSegmentationByResourceNameSegmentationByResourceName,
 )
 from .get_source import (
     GetSource,
+    GetSourceSourceAwsAthenaSource,
     GetSourceSourceAwsKinesisSource,
     GetSourceSourceAwsRedshiftSource,
     GetSourceSourceAwsS3Source,
     GetSourceSourceGcpBigQuerySource,
     GetSourceSourceGcpPubSubLiteSource,
     GetSourceSourceGcpPubSubSource,
     GetSourceSourceGcpStorageSource,
+    GetSourceSourceKafkaSource,
     GetSourceSourcePostgreSqlSource,
     GetSourceSourceSnowflakeSource,
     GetSourceSourceSource,
 )
 from .get_source_by_resource_name import (
     GetSourceByResourceName,
+    GetSourceByResourceNameSourceByResourceNameAwsAthenaSource,
     GetSourceByResourceNameSourceByResourceNameAwsKinesisSource,
     GetSourceByResourceNameSourceByResourceNameAwsRedshiftSource,
     GetSourceByResourceNameSourceByResourceNameAwsS3Source,
     GetSourceByResourceNameSourceByResourceNameGcpBigQuerySource,
     GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSource,
     GetSourceByResourceNameSourceByResourceNameGcpPubSubSource,
     GetSourceByResourceNameSourceByResourceNameGcpStorageSource,
+    GetSourceByResourceNameSourceByResourceNameKafkaSource,
     GetSourceByResourceNameSourceByResourceNamePostgreSqlSource,
     GetSourceByResourceNameSourceByResourceNameSnowflakeSource,
     GetSourceByResourceNameSourceByResourceNameSource,
 )
 from .get_source_incidents import (
     GetSourceIncidents,
     GetSourceIncidentsSourceIncidentsSchemaChangeNotification,
@@ -382,25 +413,32 @@
 from .get_window_by_resource_name import (
     GetWindowByResourceName,
     GetWindowByResourceNameWindowByResourceNameFixedBatchWindow,
     GetWindowByResourceNameWindowByResourceNameSessionizedWindow,
     GetWindowByResourceNameWindowByResourceNameTumblingWindow,
     GetWindowByResourceNameWindowByResourceNameWindow,
 )
+from .infer_aws_athena_schema import InferAwsAthenaSchema
 from .infer_aws_kinesis_schema import InferAwsKinesisSchema
 from .infer_aws_redshift_schema import InferAwsRedshiftSchema
 from .infer_aws_s3_schema import InferAwsS3Schema
 from .infer_demo_schema import InferDemoSchema
 from .infer_gcp_big_query_schema import InferGcpBigQuerySchema
 from .infer_gcp_pub_sub_lite_schema import InferGcpPubSubLiteSchema
 from .infer_gcp_pub_sub_schema import InferGcpPubSubSchema
 from .infer_gcp_storage_schema import InferGcpStorageSchema
+from .infer_kafka_schema import InferKafkaSchema
 from .infer_postgre_sql_schema import InferPostgreSqlSchema
 from .infer_snowflake_schema import InferSnowflakeSchema
 from .input_types import (
+    AwsAthenaCredentialCreateInput,
+    AwsAthenaCredentialUpdateInput,
+    AwsAthenaInferSchemaInput,
+    AwsAthenaSourceCreateInput,
+    AwsAthenaSourceUpdateInput,
     AwsCredentialCreateInput,
     AwsCredentialSecretChangedInput,
     AwsCredentialUpdateInput,
     AwsKinesisDestinationCreateInput,
     AwsKinesisDestinationUpdateInput,
     AwsKinesisInferSchemaInput,
     AwsKinesisSourceCreateInput,
@@ -442,14 +480,23 @@
     GcpPubSubSourceUpdateInput,
     GcpStorageInferSchemaInput,
     GcpStorageSourceCreateInput,
     GcpStorageSourceUpdateInput,
     IdentityDeleteInput,
     IdentityProviderDeleteInput,
     IncidentsInput,
+    KafkaInferSchemaInput,
+    KafkaSASLPlainCredentialCreateInput,
+    KafkaSASLPlainCredentialSecretChangedInput,
+    KafkaSASLPlainCredentialUpdateInput,
+    KafkaSourceCreateInput,
+    KafkaSourceUpdateInput,
+    KafkaSSLCredentialCreateInput,
+    KafkaSSLCredentialSecretChangedInput,
+    KafkaSSLCredentialUpdateInput,
     LocalIdentityProviderUpdateInput,
     MonotonicThresholdCreateInput,
     NotificationRuleCreateInput,
     NotificationRuleDeleteInput,
     NotificationRuleUpdateInput,
     NumericAnomalyValidatorCreateInput,
     NumericAnomalyValidatorUpdateInput,
@@ -464,14 +511,15 @@
     PostgreSqlSourceCreateInput,
     PostgreSqlSourceUpdateInput,
     RelativeTimeValidatorCreateInput,
     RelativeTimeValidatorUpdateInput,
     RelativeVolumeValidatorCreateInput,
     RelativeVolumeValidatorUpdateInput,
     ResourceFilter,
+    ResourceNamespaceUpdateInput,
     SamlIdentityProviderCreateInput,
     SamlIdentityProviderUpdateInput,
     SegmentationCreateInput,
     SegmentIncidentsInput,
     SessionizedWindowCreateInput,
     SessionizedWindowUpdateInput,
     SlackChannelCreateInput,
@@ -499,39 +547,52 @@
     ValidatorWithFixedThresholdUpdateInput,
     ValidatorWithMonotonicThresholdUpdateInput,
     VolumeValidatorCreateInput,
     VolumeValidatorUpdateInput,
     WebhookChannelCreateInput,
     WebhookChannelUpdateInput,
 )
+from .kafka_sasl_plain_credential_secret_changed import (
+    KafkaSaslPlainCredentialSecretChanged,
+    KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged,
+)
+from .kafka_ssl_credential_secret_changed import (
+    KafkaSslCredentialSecretChanged,
+    KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged,
+)
 from .list_credentials import (
     ListCredentials,
+    ListCredentialsCredentialsListAwsAthenaCredential,
     ListCredentialsCredentialsListAwsCredential,
     ListCredentialsCredentialsListAwsRedshiftCredential,
     ListCredentialsCredentialsListCredential,
+    ListCredentialsCredentialsListKafkaSASLPlainCredential,
+    ListCredentialsCredentialsListKafkaSSLCredential,
     ListCredentialsCredentialsListPostgreSqlCredential,
     ListCredentialsCredentialsListSnowflakeCredential,
 )
 from .list_destinations import (
     ListDestinations,
     ListDestinationsDestinationsListAwsKinesisDestination,
     ListDestinationsDestinationsListDestination,
     ListDestinationsDestinationsListGcpBigQueryDestination,
     ListDestinationsDestinationsListSnowflakeDestination,
 )
 from .list_segmentations import ListSegmentations, ListSegmentationsSegmentationsList
 from .list_sources import (
     ListSources,
+    ListSourcesSourcesListAwsAthenaSource,
     ListSourcesSourcesListAwsKinesisSource,
     ListSourcesSourcesListAwsRedshiftSource,
     ListSourcesSourcesListAwsS3Source,
     ListSourcesSourcesListGcpBigQuerySource,
     ListSourcesSourcesListGcpPubSubLiteSource,
     ListSourcesSourcesListGcpPubSubSource,
     ListSourcesSourcesListGcpStorageSource,
+    ListSourcesSourcesListKafkaSource,
     ListSourcesSourcesListPostgreSqlSource,
     ListSourcesSourcesListSnowflakeSource,
     ListSourcesSourcesListSource,
 )
 from .list_validators import (
     ListValidators,
     ListValidatorsValidatorsListCategoricalDistributionValidator,
@@ -562,14 +623,22 @@
 )
 from .snowflake_credential_secret_changed import (
     SnowflakeCredentialSecretChanged,
     SnowflakeCredentialSecretChangedSnowflakeCredentialSecretChanged,
 )
 from .start_source import StartSource, StartSourceSourceStart
 from .stop_source import StopSource, StopSourceSourceStop
+from .update_aws_athena_credential import (
+    UpdateAwsAthenaCredential,
+    UpdateAwsAthenaCredentialAwsAthenaCredentialUpdate,
+)
+from .update_aws_athena_source import (
+    UpdateAwsAthenaSource,
+    UpdateAwsAthenaSourceAwsAthenaSourceUpdate,
+)
 from .update_aws_credential import (
     UpdateAwsCredential,
     UpdateAwsCredentialAwsCredentialUpdate,
 )
 from .update_aws_kinesis_destination import (
     UpdateAwsKinesisDestination,
     UpdateAwsKinesisDestinationAwsKinesisDestinationUpdate,
@@ -587,14 +656,26 @@
     UpdateAwsRedshiftSourceAwsRedshiftSourceUpdate,
 )
 from .update_aws_s3_source import UpdateAwsS3Source, UpdateAwsS3SourceAwsS3SourceUpdate
 from .update_categorical_distribution_validator import (
     UpdateCategoricalDistributionValidator,
     UpdateCategoricalDistributionValidatorCategoricalDistributionValidatorUpdate,
 )
+from .update_channel_namespace import (
+    UpdateChannelNamespace,
+    UpdateChannelNamespaceChannelNamespaceUpdate,
+)
+from .update_credential_namespace import (
+    UpdateCredentialNamespace,
+    UpdateCredentialNamespaceCredentialNamespaceUpdate,
+)
+from .update_destination_namespace import (
+    UpdateDestinationNamespace,
+    UpdateDestinationNamespaceDestinationNamespaceUpdate,
+)
 from .update_fixed_batch_window import (
     UpdateFixedBatchWindow,
     UpdateFixedBatchWindowFixedBatchWindowUpdate,
 )
 from .update_freshness_validator import (
     UpdateFreshnessValidator,
     UpdateFreshnessValidatorFreshnessValidatorUpdate,
@@ -619,22 +700,39 @@
     UpdateGcpPubSubSource,
     UpdateGcpPubSubSourceGcpPubSubSourceUpdate,
 )
 from .update_gcp_storage_source import (
     UpdateGcpStorageSource,
     UpdateGcpStorageSourceGcpStorageSourceUpdate,
 )
+from .update_identity_provider_namespace import (
+    UpdateIdentityProviderNamespace,
+    UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate,
+)
+from .update_kafka_sasl_plain_credential import (
+    UpdateKafkaSaslPlainCredential,
+    UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate,
+)
+from .update_kafka_source import UpdateKafkaSource, UpdateKafkaSourceKafkaSourceUpdate
+from .update_kafka_ssl_credential import (
+    UpdateKafkaSslCredential,
+    UpdateKafkaSslCredentialKafkaSslCredentialUpdate,
+)
 from .update_local_identity_provider import (
     UpdateLocalIdentityProvider,
     UpdateLocalIdentityProviderLocalIdentityProviderUpdate,
 )
 from .update_notification_rule import (
     UpdateNotificationRule,
     UpdateNotificationRuleNotificationRuleUpdate,
 )
+from .update_notification_rule_namespace import (
+    UpdateNotificationRuleNamespace,
+    UpdateNotificationRuleNamespaceNotificationRuleNamespaceUpdate,
+)
 from .update_numeric_anomaly_validator import (
     UpdateNumericAnomalyValidator,
     UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate,
 )
 from .update_numeric_distribution_validator import (
     UpdateNumericDistributionValidator,
     UpdateNumericDistributionValidatorNumericDistributionValidatorUpdate,
@@ -659,14 +757,18 @@
     UpdateRelativeVolumeValidator,
     UpdateRelativeVolumeValidatorRelativeVolumeValidatorUpdate,
 )
 from .update_saml_identity_provider import (
     UpdateSamlIdentityProvider,
     UpdateSamlIdentityProviderSamlIdentityProviderUpdate,
 )
+from .update_segmentation_namespace import (
+    UpdateSegmentationNamespace,
+    UpdateSegmentationNamespaceSegmentationNamespaceUpdate,
+)
 from .update_sessionized_window import (
     UpdateSessionizedWindow,
     UpdateSessionizedWindowSessionizedWindowUpdate,
 )
 from .update_slack_channel import (
     UpdateSlackChannel,
     UpdateSlackChannelSlackChannelUpdate,
@@ -679,19 +781,31 @@
     UpdateSnowflakeDestination,
     UpdateSnowflakeDestinationSnowflakeDestinationUpdate,
 )
 from .update_snowflake_source import (
     UpdateSnowflakeSource,
     UpdateSnowflakeSourceSnowflakeSourceUpdate,
 )
+from .update_source_namespace import (
+    UpdateSourceNamespace,
+    UpdateSourceNamespaceSourceNamespaceUpdate,
+)
 from .update_tumbling_window import (
     UpdateTumblingWindow,
     UpdateTumblingWindowTumblingWindowUpdate,
 )
 from .update_user import UpdateUser, UpdateUserUserUpdate
+from .update_user_namespace import (
+    UpdateUserNamespace,
+    UpdateUserNamespaceUserNamespaceUpdate,
+)
+from .update_validator_namespace import (
+    UpdateValidatorNamespace,
+    UpdateValidatorNamespaceValidatorNamespaceUpdate,
+)
 from .update_validator_with_dynamic_threshold import (
     UpdateValidatorWithDynamicThreshold,
     UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate,
 )
 from .update_validator_with_fixed_threshold import (
     UpdateValidatorWithFixedThreshold,
     UpdateValidatorWithFixedThresholdValidatorWithFixedThresholdUpdate,
@@ -704,14 +818,18 @@
     UpdateVolumeValidator,
     UpdateVolumeValidatorVolumeValidatorUpdate,
 )
 from .update_webhook_channel import (
     UpdateWebhookChannel,
     UpdateWebhookChannelWebhookChannelUpdate,
 )
+from .update_window_namespace import (
+    UpdateWindowNamespace,
+    UpdateWindowNamespaceWindowNamespaceUpdate,
+)
 
 
 def gql(q: str) -> str:
     return q
 
 
 class Client(AsyncBaseClient):
@@ -822,14 +940,270 @@
             """
         )
         variables: dict[str, object] = {"id": id}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return BackfillSource.parse_obj(data).source_backfill
 
+    async def create_aws_athena_credential(
+        self, input: AwsAthenaCredentialCreateInput
+    ) -> CreateAwsAthenaCredentialAwsAthenaCredentialCreate:
+        query = gql(
+            """
+            mutation CreateAwsAthenaCredential($input: AwsAthenaCredentialCreateInput!) {
+              awsAthenaCredentialCreate(input: $input) {
+                ...CredentialCreation
+              }
+            }
+
+            fragment CredentialCreation on CredentialCreateResult {
+              __typename
+              errors {
+                ...ErrorDetails
+              }
+              credential {
+                ...CredentialDetails
+              }
+            }
+
+            fragment CredentialDetails on Credential {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              resourceName
+              resourceNamespace
+              ... on AwsCredential {
+                config {
+                  accessKey
+                }
+              }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
+              ... on AwsRedshiftCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on PostgreSqlCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on SnowflakeCredential {
+                config {
+                  account
+                  user
+                }
+              }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return CreateAwsAthenaCredential.parse_obj(data).aws_athena_credential_create
+
+    async def create_aws_athena_source(
+        self, input: AwsAthenaSourceCreateInput
+    ) -> CreateAwsAthenaSourceAwsAthenaSourceCreate:
+        query = gql(
+            """
+            mutation CreateAwsAthenaSource($input: AwsAthenaSourceCreateInput!) {
+              awsAthenaSourceCreate(input: $input) {
+                ...SourceCreation
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment SourceCreation on SourceCreateResult {
+              errors {
+                ...ErrorDetails
+              }
+              source {
+                ...SourceDetails
+              }
+            }
+
+            fragment SourceDetails on Source {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              credential {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              windows {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              segmentations {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              jtdSchema
+              state
+              stateUpdatedAt
+              resourceName
+              resourceNamespace
+              ... on GcpStorageSource {
+                config {
+                  project
+                  bucket
+                  folder
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on GcpBigQuerySource {
+                config {
+                  project
+                  dataset
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on GcpPubSubSource {
+                config {
+                  project
+                  subscriptionId
+                }
+              }
+              ... on GcpPubSubLiteSource {
+                config {
+                  location
+                  project
+                  subscriptionId
+                }
+              }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsKinesisSource {
+                config {
+                  region
+                  streamName
+                }
+              }
+              ... on AwsRedshiftSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsS3Source {
+                config {
+                  bucket
+                  prefix
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on PostgreSqlSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on SnowflakeSource {
+                config {
+                  role
+                  warehouse
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return CreateAwsAthenaSource.parse_obj(data).aws_athena_source_create
+
     async def create_aws_credential(
         self, input: AwsCredentialCreateInput
     ) -> CreateAwsCredentialAwsCredentialCreate:
         query = gql(
             """
             mutation CreateAwsCredential($input: AwsCredentialCreateInput!) {
               awsCredentialCreate(input: $input) {
@@ -856,14 +1230,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -878,14 +1259,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment ErrorDetails on ApiError {
               __typename
               code
               message
             }
@@ -1056,14 +1452,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -1106,14 +1512,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateAwsKinesisSource.parse_obj(data).aws_kinesis_source_create
@@ -1148,14 +1559,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -1170,14 +1588,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment ErrorDetails on ApiError {
               __typename
               code
               message
             }
@@ -1277,14 +1710,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -1327,14 +1770,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateAwsRedshiftSource.parse_obj(data).aws_redshift_source_create
@@ -1426,14 +1874,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -1476,14 +1934,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateAwsS3Source.parse_obj(data).aws_s3_source_create
@@ -2172,14 +2635,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -2194,14 +2664,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment ErrorDetails on ApiError {
               __typename
               code
               message
             }
@@ -2299,14 +2784,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -2349,14 +2844,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateDemoSource.parse_obj(data).demo_source_create
@@ -3306,14 +3806,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -3356,14 +3866,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateGcpBigQuerySource.parse_obj(data).gcp_big_query_source_create
@@ -3398,14 +3913,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -3420,14 +3942,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment ErrorDetails on ApiError {
               __typename
               code
               message
             }
@@ -3525,14 +4062,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -3575,14 +4122,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateGcpPubSubLiteSource.parse_obj(data).gcp_pub_sub_lite_source_create
@@ -3674,14 +4226,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -3724,14 +4286,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateGcpPubSubSource.parse_obj(data).gcp_pub_sub_source_create
@@ -3823,14 +4390,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -3873,22 +4450,377 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateGcpStorageSource.parse_obj(data).gcp_storage_source_create
 
+    async def create_kafka_sasl_plain_credential(
+        self, input: KafkaSASLPlainCredentialCreateInput
+    ) -> CreateKafkaSaslPlainCredentialKafkaSaslPlainCredentialCreate:
+        query = gql(
+            """
+            mutation CreateKafkaSaslPlainCredential($input: KafkaSASLPlainCredentialCreateInput!) {
+              kafkaSaslPlainCredentialCreate(input: $input) {
+                ...CredentialCreation
+              }
+            }
+
+            fragment CredentialCreation on CredentialCreateResult {
+              __typename
+              errors {
+                ...ErrorDetails
+              }
+              credential {
+                ...CredentialDetails
+              }
+            }
+
+            fragment CredentialDetails on Credential {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              resourceName
+              resourceNamespace
+              ... on AwsCredential {
+                config {
+                  accessKey
+                }
+              }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
+              ... on AwsRedshiftCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on PostgreSqlCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on SnowflakeCredential {
+                config {
+                  account
+                  user
+                }
+              }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return CreateKafkaSaslPlainCredential.parse_obj(
+            data
+        ).kafka_sasl_plain_credential_create
+
+    async def create_kafka_source(
+        self, input: KafkaSourceCreateInput
+    ) -> CreateKafkaSourceKafkaSourceCreate:
+        query = gql(
+            """
+            mutation CreateKafkaSource($input: KafkaSourceCreateInput!) {
+              kafkaSourceCreate(input: $input) {
+                ...SourceCreation
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment SourceCreation on SourceCreateResult {
+              errors {
+                ...ErrorDetails
+              }
+              source {
+                ...SourceDetails
+              }
+            }
+
+            fragment SourceDetails on Source {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              credential {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              windows {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              segmentations {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              jtdSchema
+              state
+              stateUpdatedAt
+              resourceName
+              resourceNamespace
+              ... on GcpStorageSource {
+                config {
+                  project
+                  bucket
+                  folder
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on GcpBigQuerySource {
+                config {
+                  project
+                  dataset
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on GcpPubSubSource {
+                config {
+                  project
+                  subscriptionId
+                }
+              }
+              ... on GcpPubSubLiteSource {
+                config {
+                  location
+                  project
+                  subscriptionId
+                }
+              }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsKinesisSource {
+                config {
+                  region
+                  streamName
+                }
+              }
+              ... on AwsRedshiftSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsS3Source {
+                config {
+                  bucket
+                  prefix
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on PostgreSqlSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on SnowflakeSource {
+                config {
+                  role
+                  warehouse
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return CreateKafkaSource.parse_obj(data).kafka_source_create
+
+    async def create_kafka_ssl_credential(
+        self, input: KafkaSSLCredentialCreateInput
+    ) -> CreateKafkaSslCredentialKafkaSslCredentialCreate:
+        query = gql(
+            """
+            mutation CreateKafkaSslCredential($input: KafkaSSLCredentialCreateInput!) {
+              kafkaSslCredentialCreate(input: $input) {
+                ...CredentialCreation
+              }
+            }
+
+            fragment CredentialCreation on CredentialCreateResult {
+              __typename
+              errors {
+                ...ErrorDetails
+              }
+              credential {
+                ...CredentialDetails
+              }
+            }
+
+            fragment CredentialDetails on Credential {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              resourceName
+              resourceNamespace
+              ... on AwsCredential {
+                config {
+                  accessKey
+                }
+              }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
+              ... on AwsRedshiftCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on PostgreSqlCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on SnowflakeCredential {
+                config {
+                  account
+                  user
+                }
+              }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return CreateKafkaSslCredential.parse_obj(data).kafka_ssl_credential_create
+
     async def create_notification_rule(
         self, input: NotificationRuleCreateInput
     ) -> CreateNotificationRuleNotificationRuleCreate:
         query = gql(
             """
             mutation CreateNotificationRule($input: NotificationRuleCreateInput!) {
               notificationRuleCreate(input: $input) {
@@ -6587,14 +7519,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -6609,14 +7548,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment ErrorDetails on ApiError {
               __typename
               code
               message
             }
@@ -6714,14 +7668,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -6764,14 +7728,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreatePostgreSqlSource.parse_obj(data).postgre_sql_source_create
@@ -8659,14 +9628,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -8681,14 +9657,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment ErrorDetails on ApiError {
               __typename
               code
               message
             }
@@ -8857,14 +9848,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -8907,14 +9908,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return CreateSnowflakeSource.parse_obj(data).snowflake_source_create
@@ -10327,17 +11333,20 @@
 
     async def get_credential_by_resource_name(
         self, resource_name: str, resource_namespace: str
     ) -> Optional[
         Union[
             GetCredentialByResourceNameCredentialByResourceNameCredential,
             GetCredentialByResourceNameCredentialByResourceNameAwsCredential,
+            GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential,
             GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential,
             GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential,
             GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential,
+            GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential,
+            GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential,
         ]
     ]:
         query = gql(
             """
             query GetCredentialByResourceName($resourceName: String!, $resourceNamespace: String! = "default") {
               credentialByResourceName(
                 resourceName: $resourceName
@@ -10356,14 +11365,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -10378,14 +11394,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {
             "resourceName": resource_name,
             "resourceNamespace": resource_namespace,
         }
@@ -10747,14 +11778,53 @@
             """
         )
         variables: dict[str, object] = {"filter": filter}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetNotificationRules.parse_obj(data).notification_rules
 
+    async def get_recommendation(
+        self, id: Any
+    ) -> Union[
+        GetRecommendationRecommendationRecommendation,
+        GetRecommendationRecommendationValidatorCreateRecommendation,
+        GetRecommendationRecommendationValidatorUpdateRecommendation,
+        GetRecommendationRecommendationValidatorDeleteRecommendation,
+    ]:
+        query = gql(
+            """
+            query GetRecommendation($id: RecommendationId!) {
+              recommendation(id: $id) {
+                __typename
+                ...RecommendationDetails
+              }
+            }
+
+            fragment RecommendationDetails on Recommendation {
+              id
+              description
+              createdAt
+              updatedAt
+              ... on ValidatorCreateRecommendation {
+                sourceId
+              }
+              ... on ValidatorUpdateRecommendation {
+                sourceId
+              }
+              ... on ValidatorDeleteRecommendation {
+                sourceId
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"id": id}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return GetRecommendation.parse_obj(data).recommendation
+
     async def get_segment_incidents(
         self, input: SegmentIncidentsInput
     ) -> List[GetSegmentIncidentsSegmentIncidents]:
         query = gql(
             """
             query GetSegmentIncidents($input: SegmentIncidentsInput!) {
               segmentIncidents(input: $input) {
@@ -10892,19 +11962,21 @@
     ) -> Optional[
         Union[
             GetSourceSourceSource,
             GetSourceSourceGcpStorageSource,
             GetSourceSourceGcpBigQuerySource,
             GetSourceSourceGcpPubSubSource,
             GetSourceSourceGcpPubSubLiteSource,
+            GetSourceSourceAwsAthenaSource,
             GetSourceSourceAwsKinesisSource,
             GetSourceSourceAwsRedshiftSource,
             GetSourceSourceAwsS3Source,
             GetSourceSourcePostgreSqlSource,
             GetSourceSourceSnowflakeSource,
+            GetSourceSourceKafkaSource,
         ]
     ]:
         query = gql(
             """
             query GetSource($id: SourceId!) {
               source(id: $id) {
                 ...SourceDetails
@@ -10972,14 +12044,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -11022,14 +12104,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"id": id}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetSource.parse_obj(data).source
@@ -11039,19 +12126,21 @@
     ) -> Optional[
         Union[
             GetSourceByResourceNameSourceByResourceNameSource,
             GetSourceByResourceNameSourceByResourceNameGcpStorageSource,
             GetSourceByResourceNameSourceByResourceNameGcpBigQuerySource,
             GetSourceByResourceNameSourceByResourceNameGcpPubSubSource,
             GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSource,
+            GetSourceByResourceNameSourceByResourceNameAwsAthenaSource,
             GetSourceByResourceNameSourceByResourceNameAwsKinesisSource,
             GetSourceByResourceNameSourceByResourceNameAwsRedshiftSource,
             GetSourceByResourceNameSourceByResourceNameAwsS3Source,
             GetSourceByResourceNameSourceByResourceNamePostgreSqlSource,
             GetSourceByResourceNameSourceByResourceNameSnowflakeSource,
+            GetSourceByResourceNameSourceByResourceNameKafkaSource,
         ]
     ]:
         query = gql(
             """
             query GetSourceByResourceName($resourceName: String!, $resourceNamespace: String! = "default") {
               sourceByResourceName(
                 resourceName: $resourceName
@@ -11122,14 +12211,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -11172,14 +12271,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {
             "resourceName": resource_name,
             "resourceNamespace": resource_namespace,
         }
@@ -11260,14 +12364,18 @@
               updatedAt
               state
               progress {
                 percentage
                 processed
                 total
               }
+              stats {
+                lastArtifactAt
+                lastIncidentAt
+              }
               stateUpdatedAt
               sourceConfig {
                 source {
                   id
                 }
                 segmentation {
                   ...SegmentationSummary
@@ -12309,14 +13417,29 @@
             "resourceName": resource_name,
             "resourceNamespace": resource_namespace,
         }
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return GetWindowByResourceName.parse_obj(data).window_by_resource_name
 
+    async def infer_aws_athena_schema(
+        self, input: AwsAthenaInferSchemaInput
+    ) -> JsonTypeDefinition:
+        query = gql(
+            """
+            query InferAwsAthenaSchema($input: AwsAthenaInferSchemaInput!) {
+              awsAthenaInferSchema(input: $input)
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return InferAwsAthenaSchema.parse_obj(data).aws_athena_infer_schema
+
     async def infer_aws_kinesis_schema(
         self, input: AwsKinesisInferSchemaInput
     ) -> JsonTypeDefinition:
         query = gql(
             """
             query InferAwsKinesisSchema($input: AwsKinesisInferSchemaInput!) {
               awsKinesisInferSchema(input: $input)
@@ -12427,14 +13550,29 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return InferGcpStorageSchema.parse_obj(data).gcp_storage_infer_schema
 
+    async def infer_kafka_schema(
+        self, input: KafkaInferSchemaInput
+    ) -> JsonTypeDefinition:
+        query = gql(
+            """
+            query InferKafkaSchema($input: KafkaInferSchemaInput!) {
+              kafkaInferSchema(input: $input)
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return InferKafkaSchema.parse_obj(data).kafka_infer_schema
+
     async def infer_postgre_sql_schema(
         self, input: PostgreSqlInferSchemaInput
     ) -> JsonTypeDefinition:
         query = gql(
             """
             query InferPostgreSqlSchema($input: PostgreSqlInferSchemaInput!) {
               postgreSqlInferSchema(input: $input)
@@ -12457,23 +13595,90 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return InferSnowflakeSchema.parse_obj(data).snowflake_infer_schema
 
+    async def kafka_sasl_plain_credential_secret_changed(
+        self, input: KafkaSASLPlainCredentialSecretChangedInput
+    ) -> KafkaSaslPlainCredentialSecretChangedKafkaSaslPlainCredentialSecretChanged:
+        query = gql(
+            """
+            query KafkaSaslPlainCredentialSecretChanged($input: KafkaSASLPlainCredentialSecretChangedInput!) {
+              kafkaSaslPlainCredentialSecretChanged(input: $input) {
+                ...CredentialSecretChanged
+              }
+            }
+
+            fragment CredentialSecretChanged on CredentialSecretChangedResult {
+              errors {
+                ...ErrorDetails
+              }
+              hasChanged
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return KafkaSaslPlainCredentialSecretChanged.parse_obj(
+            data
+        ).kafka_sasl_plain_credential_secret_changed
+
+    async def kafka_ssl_credential_secret_changed(
+        self, input: KafkaSSLCredentialSecretChangedInput
+    ) -> KafkaSslCredentialSecretChangedKafkaSslCredentialSecretChanged:
+        query = gql(
+            """
+            query KafkaSslCredentialSecretChanged($input: KafkaSSLCredentialSecretChangedInput!) {
+              kafkaSslCredentialSecretChanged(input: $input) {
+                ...CredentialSecretChanged
+              }
+            }
+
+            fragment CredentialSecretChanged on CredentialSecretChangedResult {
+              errors {
+                ...ErrorDetails
+              }
+              hasChanged
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return KafkaSslCredentialSecretChanged.parse_obj(
+            data
+        ).kafka_ssl_credential_secret_changed
+
     async def list_credentials(
         self, filter: Union[Optional[ResourceFilter], UnsetType] = UNSET
     ) -> List[
         Union[
             ListCredentialsCredentialsListCredential,
             ListCredentialsCredentialsListAwsCredential,
+            ListCredentialsCredentialsListAwsAthenaCredential,
             ListCredentialsCredentialsListAwsRedshiftCredential,
             ListCredentialsCredentialsListPostgreSqlCredential,
             ListCredentialsCredentialsListSnowflakeCredential,
+            ListCredentialsCredentialsListKafkaSSLCredential,
+            ListCredentialsCredentialsListKafkaSASLPlainCredential,
         ]
     ]:
         query = gql(
             """
             query ListCredentials($filter: ResourceFilter) {
               credentialsList(filter: $filter) {
                 ...CredentialDetails
@@ -12489,14 +13694,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -12511,14 +13723,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"filter": filter}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return ListCredentials.parse_obj(data).credentials_list
@@ -12625,19 +13852,21 @@
     ) -> List[
         Union[
             ListSourcesSourcesListSource,
             ListSourcesSourcesListGcpStorageSource,
             ListSourcesSourcesListGcpBigQuerySource,
             ListSourcesSourcesListGcpPubSubSource,
             ListSourcesSourcesListGcpPubSubLiteSource,
+            ListSourcesSourcesListAwsAthenaSource,
             ListSourcesSourcesListAwsKinesisSource,
             ListSourcesSourcesListAwsRedshiftSource,
             ListSourcesSourcesListAwsS3Source,
             ListSourcesSourcesListPostgreSqlSource,
             ListSourcesSourcesListSnowflakeSource,
+            ListSourcesSourcesListKafkaSource,
         ]
     ]:
         query = gql(
             """
             query ListSources($filter: ResourceFilter) {
               sourcesList(filter: $filter) {
                 ...SourceDetails
@@ -12705,14 +13934,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -12755,14 +13994,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
             """
         )
         variables: dict[str, object] = {"filter": filter}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return ListSources.parse_obj(data).sources_list
@@ -13310,14 +14554,269 @@
             """
         )
         variables: dict[str, object] = {"id": id}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return StopSource.parse_obj(data).source_stop
 
+    async def update_aws_athena_credential(
+        self, input: AwsAthenaCredentialUpdateInput
+    ) -> UpdateAwsAthenaCredentialAwsAthenaCredentialUpdate:
+        query = gql(
+            """
+            mutation UpdateAwsAthenaCredential($input: AwsAthenaCredentialUpdateInput!) {
+              awsAthenaCredentialUpdate(input: $input) {
+                ...CredentialUpdate
+              }
+            }
+
+            fragment CredentialDetails on Credential {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              resourceName
+              resourceNamespace
+              ... on AwsCredential {
+                config {
+                  accessKey
+                }
+              }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
+              ... on AwsRedshiftCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on PostgreSqlCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on SnowflakeCredential {
+                config {
+                  account
+                  user
+                }
+              }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
+            }
+
+            fragment CredentialUpdate on CredentialUpdateResult {
+              errors {
+                ...ErrorDetails
+              }
+              credential {
+                ...CredentialDetails
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateAwsAthenaCredential.parse_obj(data).aws_athena_credential_update
+
+    async def update_aws_athena_source(
+        self, input: AwsAthenaSourceUpdateInput
+    ) -> UpdateAwsAthenaSourceAwsAthenaSourceUpdate:
+        query = gql(
+            """
+            mutation UpdateAwsAthenaSource($input: AwsAthenaSourceUpdateInput!) {
+              awsAthenaSourceUpdate(input: $input) {
+                ...SourceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment SourceDetails on Source {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              credential {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              windows {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              segmentations {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              jtdSchema
+              state
+              stateUpdatedAt
+              resourceName
+              resourceNamespace
+              ... on GcpStorageSource {
+                config {
+                  project
+                  bucket
+                  folder
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on GcpBigQuerySource {
+                config {
+                  project
+                  dataset
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on GcpPubSubSource {
+                config {
+                  project
+                  subscriptionId
+                }
+              }
+              ... on GcpPubSubLiteSource {
+                config {
+                  location
+                  project
+                  subscriptionId
+                }
+              }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsKinesisSource {
+                config {
+                  region
+                  streamName
+                }
+              }
+              ... on AwsRedshiftSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsS3Source {
+                config {
+                  bucket
+                  prefix
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on PostgreSqlSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on SnowflakeSource {
+                config {
+                  role
+                  warehouse
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
+            }
+
+            fragment SourceUpdate on SourceUpdateResult {
+              errors {
+                ...ErrorDetails
+              }
+              source {
+                ...SourceDetails
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateAwsAthenaSource.parse_obj(data).aws_athena_source_update
+
     async def update_aws_credential(
         self, input: AwsCredentialUpdateInput
     ) -> UpdateAwsCredentialAwsCredentialUpdate:
         query = gql(
             """
             mutation UpdateAwsCredential($input: AwsCredentialUpdateInput!) {
               awsCredentialUpdate(input: $input) {
@@ -13334,14 +14833,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -13356,14 +14862,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment CredentialUpdate on CredentialUpdateResult {
               errors {
                 ...ErrorDetails
               }
               credential {
@@ -13534,14 +15055,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -13584,14 +15115,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -13625,14 +15161,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -13647,14 +15190,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment CredentialUpdate on CredentialUpdateResult {
               errors {
                 ...ErrorDetails
               }
               credential {
@@ -13754,14 +15312,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -13804,14 +15372,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -13903,14 +15476,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -13953,14 +15536,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -14292,14 +15880,107 @@
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateCategoricalDistributionValidator.parse_obj(
             data
         ).categorical_distribution_validator_update
 
+    async def update_channel_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateChannelNamespaceChannelNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateChannelNamespace($input: ResourceNamespaceUpdateInput!) {
+              channelNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateChannelNamespace.parse_obj(data).channel_namespace_update
+
+    async def update_credential_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateCredentialNamespaceCredentialNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateCredentialNamespace($input: ResourceNamespaceUpdateInput!) {
+              credentialNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateCredentialNamespace.parse_obj(data).credential_namespace_update
+
+    async def update_destination_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateDestinationNamespaceDestinationNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateDestinationNamespace($input: ResourceNamespaceUpdateInput!) {
+              destinationNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateDestinationNamespace.parse_obj(data).destination_namespace_update
+
     async def update_fixed_batch_window(
         self, input: FixedBatchWindowUpdateInput
     ) -> UpdateFixedBatchWindowFixedBatchWindowUpdate:
         query = gql(
             """
             mutation UpdateFixedBatchWindow($input: FixedBatchWindowUpdateInput!) {
               fixedBatchWindowUpdate(input: $input) {
@@ -14835,14 +16516,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -14885,14 +16576,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -14926,14 +16622,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -14948,14 +16651,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment CredentialUpdate on CredentialUpdateResult {
               errors {
                 ...ErrorDetails
               }
               credential {
@@ -15053,14 +16771,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -15103,14 +16831,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -15202,14 +16935,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -15252,14 +16995,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -15351,14 +17099,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -15401,14 +17159,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -15418,14 +17181,395 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateGcpStorageSource.parse_obj(data).gcp_storage_source_update
 
+    async def update_identity_provider_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateIdentityProviderNamespaceIdentityProviderNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateIdentityProviderNamespace($input: ResourceNamespaceUpdateInput!) {
+              identityProviderNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateIdentityProviderNamespace.parse_obj(
+            data
+        ).identity_provider_namespace_update
+
+    async def update_kafka_sasl_plain_credential(
+        self, input: KafkaSASLPlainCredentialUpdateInput
+    ) -> UpdateKafkaSaslPlainCredentialKafkaSaslPlainCredentialUpdate:
+        query = gql(
+            """
+            mutation UpdateKafkaSaslPlainCredential($input: KafkaSASLPlainCredentialUpdateInput!) {
+              kafkaSaslPlainCredentialUpdate(input: $input) {
+                ...CredentialUpdate
+              }
+            }
+
+            fragment CredentialDetails on Credential {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              resourceName
+              resourceNamespace
+              ... on AwsCredential {
+                config {
+                  accessKey
+                }
+              }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
+              ... on AwsRedshiftCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on PostgreSqlCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on SnowflakeCredential {
+                config {
+                  account
+                  user
+                }
+              }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
+            }
+
+            fragment CredentialUpdate on CredentialUpdateResult {
+              errors {
+                ...ErrorDetails
+              }
+              credential {
+                ...CredentialDetails
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateKafkaSaslPlainCredential.parse_obj(
+            data
+        ).kafka_sasl_plain_credential_update
+
+    async def update_kafka_source(
+        self, input: KafkaSourceUpdateInput
+    ) -> UpdateKafkaSourceKafkaSourceUpdate:
+        query = gql(
+            """
+            mutation UpdateKafkaSource($input: KafkaSourceUpdateInput!) {
+              kafkaSourceUpdate(input: $input) {
+                ...SourceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment SourceDetails on Source {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              credential {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              windows {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              segmentations {
+                id
+                name
+                resourceName
+                resourceNamespace
+              }
+              jtdSchema
+              state
+              stateUpdatedAt
+              resourceName
+              resourceNamespace
+              ... on GcpStorageSource {
+                config {
+                  project
+                  bucket
+                  folder
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on GcpBigQuerySource {
+                config {
+                  project
+                  dataset
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on GcpPubSubSource {
+                config {
+                  project
+                  subscriptionId
+                }
+              }
+              ... on GcpPubSubLiteSource {
+                config {
+                  location
+                  project
+                  subscriptionId
+                }
+              }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsKinesisSource {
+                config {
+                  region
+                  streamName
+                }
+              }
+              ... on AwsRedshiftSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on AwsS3Source {
+                config {
+                  bucket
+                  prefix
+                  csv {
+                    nullMarker
+                    delimiter
+                  }
+                  schedule
+                  filePattern
+                }
+              }
+              ... on PostgreSqlSource {
+                config {
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on SnowflakeSource {
+                config {
+                  role
+                  warehouse
+                  database
+                  schema
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
+            }
+
+            fragment SourceUpdate on SourceUpdateResult {
+              errors {
+                ...ErrorDetails
+              }
+              source {
+                ...SourceDetails
+              }
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateKafkaSource.parse_obj(data).kafka_source_update
+
+    async def update_kafka_ssl_credential(
+        self, input: KafkaSSLCredentialUpdateInput
+    ) -> UpdateKafkaSslCredentialKafkaSslCredentialUpdate:
+        query = gql(
+            """
+            mutation UpdateKafkaSslCredential($input: KafkaSSLCredentialUpdateInput!) {
+              kafkaSslCredentialUpdate(input: $input) {
+                ...CredentialUpdate
+              }
+            }
+
+            fragment CredentialDetails on Credential {
+              __typename
+              id
+              name
+              createdAt
+              updatedAt
+              resourceName
+              resourceNamespace
+              ... on AwsCredential {
+                config {
+                  accessKey
+                }
+              }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
+              ... on AwsRedshiftCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on PostgreSqlCredential {
+                config {
+                  host
+                  port
+                  user
+                  defaultDatabase
+                }
+              }
+              ... on SnowflakeCredential {
+                config {
+                  account
+                  user
+                }
+              }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
+            }
+
+            fragment CredentialUpdate on CredentialUpdateResult {
+              errors {
+                ...ErrorDetails
+              }
+              credential {
+                ...CredentialDetails
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateKafkaSslCredential.parse_obj(data).kafka_ssl_credential_update
+
     async def update_local_identity_provider(
         self, input: LocalIdentityProviderUpdateInput
     ) -> UpdateLocalIdentityProviderLocalIdentityProviderUpdate:
         query = gql(
             """
             mutation UpdateLocalIdentityProvider($input: LocalIdentityProviderUpdateInput!) {
               localIdentityProviderUpdate(input: $input) {
@@ -15531,14 +17675,47 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateNotificationRule.parse_obj(data).notification_rule_update
 
+    async def update_notification_rule_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateNotificationRuleNamespaceNotificationRuleNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateNotificationRuleNamespace($input: ResourceNamespaceUpdateInput!) {
+              notificationRuleNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateNotificationRuleNamespace.parse_obj(
+            data
+        ).notification_rule_namespace_update
+
     async def update_numeric_anomaly_validator(
         self, input: NumericAnomalyValidatorUpdateInput
     ) -> UpdateNumericAnomalyValidatorNumericAnomalyValidatorUpdate:
         query = gql(
             """
             mutation UpdateNumericAnomalyValidator($input: NumericAnomalyValidatorUpdateInput!) {
               numericAnomalyValidatorUpdate(input: $input) {
@@ -16519,14 +18696,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -16541,14 +18725,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment CredentialUpdate on CredentialUpdateResult {
               errors {
                 ...ErrorDetails
               }
               credential {
@@ -16646,14 +18845,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -16696,14 +18905,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -17402,14 +19616,45 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateSamlIdentityProvider.parse_obj(data).saml_identity_provider_update
 
+    async def update_segmentation_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateSegmentationNamespaceSegmentationNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateSegmentationNamespace($input: ResourceNamespaceUpdateInput!) {
+              segmentationNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateSegmentationNamespace.parse_obj(data).segmentation_namespace_update
+
     async def update_sessionized_window(
         self, input: SessionizedWindowUpdateInput
     ) -> UpdateSessionizedWindowSessionizedWindowUpdate:
         query = gql(
             """
             mutation UpdateSessionizedWindow($input: SessionizedWindowUpdateInput!) {
               sessionizedWindowUpdate(input: $input) {
@@ -17545,14 +19790,21 @@
               resourceName
               resourceNamespace
               ... on AwsCredential {
                 config {
                   accessKey
                 }
               }
+              ... on AwsAthenaCredential {
+                config {
+                  accessKey
+                  region
+                  queryResultLocation
+                }
+              }
               ... on AwsRedshiftCredential {
                 config {
                   host
                   port
                   user
                   defaultDatabase
                 }
@@ -17567,14 +19819,29 @@
               }
               ... on SnowflakeCredential {
                 config {
                   account
                   user
                 }
               }
+              ... on KafkaSSLCredential {
+                config {
+                  bootstrapServers
+                  caCertificate
+                  certificate
+                  keyPassword
+                }
+              }
+              ... on KafkaSASLPlainCredential {
+                config {
+                  bootstrapServers
+                  username
+                  password
+                }
+              }
             }
 
             fragment CredentialUpdate on CredentialUpdateResult {
               errors {
                 ...ErrorDetails
               }
               credential {
@@ -17743,14 +20010,24 @@
               ... on GcpPubSubLiteSource {
                 config {
                   location
                   project
                   subscriptionId
                 }
               }
+              ... on AwsAthenaSource {
+                config {
+                  catalog
+                  database
+                  table
+                  cursorField
+                  lookbackDays
+                  schedule
+                }
+              }
               ... on AwsKinesisSource {
                 config {
                   region
                   streamName
                 }
               }
               ... on AwsRedshiftSource {
@@ -17793,14 +20070,19 @@
                   schema
                   table
                   cursorField
                   lookbackDays
                   schedule
                 }
               }
+              ... on KafkaSource {
+                config {
+                  topic
+                }
+              }
             }
 
             fragment SourceUpdate on SourceUpdateResult {
               errors {
                 ...ErrorDetails
               }
               source {
@@ -17810,14 +20092,45 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateSnowflakeSource.parse_obj(data).snowflake_source_update
 
+    async def update_source_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateSourceNamespaceSourceNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateSourceNamespace($input: ResourceNamespaceUpdateInput!) {
+              sourceNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateSourceNamespace.parse_obj(data).source_namespace_update
+
     async def update_tumbling_window(
         self, input: TumblingWindowUpdateInput
     ) -> UpdateTumblingWindowTumblingWindowUpdate:
         query = gql(
             """
             mutation UpdateTumblingWindow($input: TumblingWindowUpdateInput!) {
               tumblingWindowUpdate(input: $input) {
@@ -17940,14 +20253,76 @@
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateUser.parse_obj(data).user_update
 
+    async def update_user_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateUserNamespaceUserNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateUserNamespace($input: ResourceNamespaceUpdateInput!) {
+              userNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateUserNamespace.parse_obj(data).user_namespace_update
+
+    async def update_validator_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateValidatorNamespaceValidatorNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateValidatorNamespace($input: ResourceNamespaceUpdateInput!) {
+              validatorNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateValidatorNamespace.parse_obj(data).validator_namespace_update
+
     async def update_validator_with_dynamic_threshold(
         self, input: ValidatorWithDynamicThresholdUpdateInput
     ) -> UpdateValidatorWithDynamicThresholdValidatorWithDynamicThresholdUpdate:
         query = gql(
             """
             mutation UpdateValidatorWithDynamicThreshold($input: ValidatorWithDynamicThresholdUpdateInput!) {
               validatorWithDynamicThresholdUpdate(input: $input) {
@@ -19264,7 +21639,38 @@
             }
             """
         )
         variables: dict[str, object] = {"input": input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UpdateWebhookChannel.parse_obj(data).webhook_channel_update
+
+    async def update_window_namespace(
+        self, input: ResourceNamespaceUpdateInput
+    ) -> UpdateWindowNamespaceWindowNamespaceUpdate:
+        query = gql(
+            """
+            mutation UpdateWindowNamespace($input: ResourceNamespaceUpdateInput!) {
+              windowNamespaceUpdate(input: $input) {
+                ...NamespaceUpdate
+              }
+            }
+
+            fragment ErrorDetails on ApiError {
+              __typename
+              code
+              message
+            }
+
+            fragment NamespaceUpdate on ResourceNamespaceUpdatedResult {
+              errors {
+                ...ErrorDetails
+              }
+              resourceName
+              resourceNamespace
+            }
+            """
+        )
+        variables: dict[str, object] = {"input": input}
+        response = await self.execute(query=query, variables=variables)
+        data = self.get_data(response)
+        return UpdateWindowNamespace.parse_obj(data).window_namespace_update
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_kinesis_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_aws_redshift_credential.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_categorical_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_freshness_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_gcp_big_query_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_anomaly_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_distribution_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_numeric_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_postgre_sql_credential.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_time_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_relative_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_saml_identity_provider.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_snowflake_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/create_volume_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_credential.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_credentials.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_destinations.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_segmentation.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_segmentation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_source.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_sources.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_sources.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_validators.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_window.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_window.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/delete_windows.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/delete_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/dismiss_validator_recommendation.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/dismiss_validator_recommendation.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/enums.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,17 @@
 class NotificationSeverity(str, Enum):
     ERROR = "ERROR"
     INFO = "INFO"
     WARNING = "WARNING"
 
 
 class NotificationTypename(str, Enum):
-    CredentialFailureNotification = "CredentialFailureNotification"
     SchemaChangeNotification = "SchemaChangeNotification"
+    SegmentLimitExceededNotification = "SegmentLimitExceededNotification"
+    SourceErrorNotification = "SourceErrorNotification"
     ValidatorThresholdFailureNotification = "ValidatorThresholdFailureNotification"
 
 
 class NumericAnomalyMetric(str, Enum):
     COUNT = "COUNT"
     PERCENTAGE = "PERCENTAGE"
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/exceptions.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/fragments.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,17 +197,20 @@
     typename__: str = Field(alias="__typename")
     errors: List["CredentialCreationErrors"]
     credential: Optional[
         Annotated[
             Union[
                 "CredentialCreationCredentialCredential",
                 "CredentialCreationCredentialAwsCredential",
+                "CredentialCreationCredentialAwsAthenaCredential",
                 "CredentialCreationCredentialAwsRedshiftCredential",
                 "CredentialCreationCredentialPostgreSqlCredential",
                 "CredentialCreationCredentialSnowflakeCredential",
+                "CredentialCreationCredentialKafkaSSLCredential",
+                "CredentialCreationCredentialKafkaSASLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class CredentialCreationErrors(ErrorDetails):
@@ -237,14 +240,31 @@
     config: "CredentialCreationCredentialAwsCredentialConfig"
 
 
 class CredentialCreationCredentialAwsCredentialConfig(BaseModel):
     access_key: str = Field(alias="accessKey")
 
 
+class CredentialCreationCredentialAwsAthenaCredential(BaseModel):
+    typename__: Literal["AwsAthenaCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "CredentialCreationCredentialAwsAthenaCredentialConfig"
+
+
+class CredentialCreationCredentialAwsAthenaCredentialConfig(BaseModel):
+    access_key: str = Field(alias="accessKey")
+    region: str
+    query_result_location: str = Field(alias="queryResultLocation")
+
+
 class CredentialCreationCredentialAwsRedshiftCredential(BaseModel):
     typename__: Literal["AwsRedshiftCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
@@ -289,14 +309,49 @@
 
 
 class CredentialCreationCredentialSnowflakeCredentialConfig(BaseModel):
     account: str
     user: str
 
 
+class CredentialCreationCredentialKafkaSSLCredential(BaseModel):
+    typename__: Literal["KafkaSSLCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "CredentialCreationCredentialKafkaSSLCredentialConfig"
+
+
+class CredentialCreationCredentialKafkaSSLCredentialConfig(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    ca_certificate: str = Field(alias="caCertificate")
+    certificate: str
+    key_password: str = Field(alias="keyPassword")
+
+
+class CredentialCreationCredentialKafkaSASLPlainCredential(BaseModel):
+    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "CredentialCreationCredentialKafkaSASLPlainCredentialConfig"
+
+
+class CredentialCreationCredentialKafkaSASLPlainCredentialConfig(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    username: str
+    password: str
+
+
 class CredentialSecretChanged(BaseModel):
     errors: List["CredentialSecretChangedErrors"]
     has_changed: Optional[bool] = Field(alias="hasChanged")
 
 
 class CredentialSecretChangedErrors(ErrorDetails):
     pass
@@ -305,17 +360,20 @@
 class CredentialUpdate(BaseModel):
     errors: List["CredentialUpdateErrors"]
     credential: Optional[
         Annotated[
             Union[
                 "CredentialUpdateCredentialCredential",
                 "CredentialUpdateCredentialAwsCredential",
+                "CredentialUpdateCredentialAwsAthenaCredential",
                 "CredentialUpdateCredentialAwsRedshiftCredential",
                 "CredentialUpdateCredentialPostgreSqlCredential",
                 "CredentialUpdateCredentialSnowflakeCredential",
+                "CredentialUpdateCredentialKafkaSSLCredential",
+                "CredentialUpdateCredentialKafkaSASLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class CredentialUpdateErrors(ErrorDetails):
@@ -345,14 +403,31 @@
     config: "CredentialUpdateCredentialAwsCredentialConfig"
 
 
 class CredentialUpdateCredentialAwsCredentialConfig(BaseModel):
     access_key: str = Field(alias="accessKey")
 
 
+class CredentialUpdateCredentialAwsAthenaCredential(BaseModel):
+    typename__: Literal["AwsAthenaCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "CredentialUpdateCredentialAwsAthenaCredentialConfig"
+
+
+class CredentialUpdateCredentialAwsAthenaCredentialConfig(BaseModel):
+    access_key: str = Field(alias="accessKey")
+    region: str
+    query_result_location: str = Field(alias="queryResultLocation")
+
+
 class CredentialUpdateCredentialAwsRedshiftCredential(BaseModel):
     typename__: Literal["AwsRedshiftCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
@@ -397,14 +472,49 @@
 
 
 class CredentialUpdateCredentialSnowflakeCredentialConfig(BaseModel):
     account: str
     user: str
 
 
+class CredentialUpdateCredentialKafkaSSLCredential(BaseModel):
+    typename__: Literal["KafkaSSLCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "CredentialUpdateCredentialKafkaSSLCredentialConfig"
+
+
+class CredentialUpdateCredentialKafkaSSLCredentialConfig(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    ca_certificate: str = Field(alias="caCertificate")
+    certificate: str
+    key_password: str = Field(alias="keyPassword")
+
+
+class CredentialUpdateCredentialKafkaSASLPlainCredential(BaseModel):
+    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "CredentialUpdateCredentialKafkaSASLPlainCredentialConfig"
+
+
+class CredentialUpdateCredentialKafkaSASLPlainCredentialConfig(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    username: str
+    password: str
+
+
 class DestinationCreation(BaseModel):
     errors: List["DestinationCreationErrors"]
     destination: Optional[
         Annotated[
             Union[
                 "DestinationCreationDestinationDestination",
                 "DestinationCreationDestinationGcpBigQueryDestination",
@@ -737,14 +847,24 @@
 
 class IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig(BaseModel):
     entry_point: str = Field(alias="entryPoint")
     entity_id: str = Field(alias="entityId")
     cert: str
 
 
+class NamespaceUpdate(BaseModel):
+    errors: List["NamespaceUpdateErrors"]
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+
+
+class NamespaceUpdateErrors(ErrorDetails):
+    pass
+
+
 class NotificationRuleDetails(BaseModel):
     typename__: str = Field(alias="__typename")
     id: Any
     name: str
     notification_typenames: List[NotificationTypename] = Field(
         alias="notificationTypenames"
     )
@@ -935,19 +1055,21 @@
         Annotated[
             Union[
                 "SourceCreationSourceSource",
                 "SourceCreationSourceGcpStorageSource",
                 "SourceCreationSourceGcpBigQuerySource",
                 "SourceCreationSourceGcpPubSubSource",
                 "SourceCreationSourceGcpPubSubLiteSource",
+                "SourceCreationSourceAwsAthenaSource",
                 "SourceCreationSourceAwsKinesisSource",
                 "SourceCreationSourceAwsRedshiftSource",
                 "SourceCreationSourceAwsS3Source",
                 "SourceCreationSourcePostgreSqlSource",
                 "SourceCreationSourceSnowflakeSource",
+                "SourceCreationSourceKafkaSource",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class SourceCreationErrors(ErrorDetails):
@@ -1173,14 +1295,61 @@
 
 class SourceCreationSourceGcpPubSubLiteSourceConfig(BaseModel):
     location: str
     project: str
     subscription_id: str = Field(alias="subscriptionId")
 
 
+class SourceCreationSourceAwsAthenaSource(BaseModel):
+    typename__: Literal["AwsAthenaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "SourceCreationSourceAwsAthenaSourceCredential"
+    windows: List["SourceCreationSourceAwsAthenaSourceWindows"]
+    segmentations: List["SourceCreationSourceAwsAthenaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "SourceCreationSourceAwsAthenaSourceConfig"
+
+
+class SourceCreationSourceAwsAthenaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceCreationSourceAwsAthenaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceCreationSourceAwsAthenaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceCreationSourceAwsAthenaSourceConfig(BaseModel):
+    catalog: str
+    database: str
+    table: str
+    cursor_field: str = Field(alias="cursorField")
+    lookback_days: int = Field(alias="lookbackDays")
+    schedule: CronExpression
+
+
 class SourceCreationSourceAwsKinesisSource(BaseModel):
     typename__: Literal["AwsKinesisSource"] = Field(alias="__typename")
     id: SourceId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     credential: "SourceCreationSourceAwsKinesisSourceCredential"
@@ -1410,29 +1579,73 @@
     db_schema: Any = Field(alias="schema")
     table: str
     cursor_field: str = Field(alias="cursorField")
     lookback_days: int = Field(alias="lookbackDays")
     schedule: CronExpression
 
 
+class SourceCreationSourceKafkaSource(BaseModel):
+    typename__: Literal["KafkaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "SourceCreationSourceKafkaSourceCredential"
+    windows: List["SourceCreationSourceKafkaSourceWindows"]
+    segmentations: List["SourceCreationSourceKafkaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "SourceCreationSourceKafkaSourceConfig"
+
+
+class SourceCreationSourceKafkaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceCreationSourceKafkaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceCreationSourceKafkaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceCreationSourceKafkaSourceConfig(BaseModel):
+    topic: str
+
+
 class SourceUpdate(BaseModel):
     errors: List["SourceUpdateErrors"]
     source: Optional[
         Annotated[
             Union[
                 "SourceUpdateSourceSource",
                 "SourceUpdateSourceGcpStorageSource",
                 "SourceUpdateSourceGcpBigQuerySource",
                 "SourceUpdateSourceGcpPubSubSource",
                 "SourceUpdateSourceGcpPubSubLiteSource",
+                "SourceUpdateSourceAwsAthenaSource",
                 "SourceUpdateSourceAwsKinesisSource",
                 "SourceUpdateSourceAwsRedshiftSource",
                 "SourceUpdateSourceAwsS3Source",
                 "SourceUpdateSourcePostgreSqlSource",
                 "SourceUpdateSourceSnowflakeSource",
+                "SourceUpdateSourceKafkaSource",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class SourceUpdateErrors(ErrorDetails):
@@ -1658,14 +1871,61 @@
 
 class SourceUpdateSourceGcpPubSubLiteSourceConfig(BaseModel):
     location: str
     project: str
     subscription_id: str = Field(alias="subscriptionId")
 
 
+class SourceUpdateSourceAwsAthenaSource(BaseModel):
+    typename__: Literal["AwsAthenaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "SourceUpdateSourceAwsAthenaSourceCredential"
+    windows: List["SourceUpdateSourceAwsAthenaSourceWindows"]
+    segmentations: List["SourceUpdateSourceAwsAthenaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "SourceUpdateSourceAwsAthenaSourceConfig"
+
+
+class SourceUpdateSourceAwsAthenaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceUpdateSourceAwsAthenaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceUpdateSourceAwsAthenaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceUpdateSourceAwsAthenaSourceConfig(BaseModel):
+    catalog: str
+    database: str
+    table: str
+    cursor_field: str = Field(alias="cursorField")
+    lookback_days: int = Field(alias="lookbackDays")
+    schedule: CronExpression
+
+
 class SourceUpdateSourceAwsKinesisSource(BaseModel):
     typename__: Literal["AwsKinesisSource"] = Field(alias="__typename")
     id: SourceId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     credential: "SourceUpdateSourceAwsKinesisSourceCredential"
@@ -1895,14 +2155,56 @@
     db_schema: Any = Field(alias="schema")
     table: str
     cursor_field: str = Field(alias="cursorField")
     lookback_days: int = Field(alias="lookbackDays")
     schedule: CronExpression
 
 
+class SourceUpdateSourceKafkaSource(BaseModel):
+    typename__: Literal["KafkaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "SourceUpdateSourceKafkaSourceCredential"
+    windows: List["SourceUpdateSourceKafkaSourceWindows"]
+    segmentations: List["SourceUpdateSourceKafkaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "SourceUpdateSourceKafkaSourceConfig"
+
+
+class SourceUpdateSourceKafkaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceUpdateSourceKafkaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceUpdateSourceKafkaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class SourceUpdateSourceKafkaSourceConfig(BaseModel):
+    topic: str
+
+
 class UserDetails(BaseModel):
     id: str
     display_name: str = Field(alias="displayName")
     full_name: Optional[str] = Field(alias="fullName")
     email: Optional[str]
     role: Role
     status: UserStatus
@@ -4025,33 +4327,45 @@
 ChannelUpdateChannelWebhookChannel.update_forward_refs()
 ChannelUpdateChannelWebhookChannelConfig.update_forward_refs()
 CredentialCreation.update_forward_refs()
 CredentialCreationErrors.update_forward_refs()
 CredentialCreationCredentialCredential.update_forward_refs()
 CredentialCreationCredentialAwsCredential.update_forward_refs()
 CredentialCreationCredentialAwsCredentialConfig.update_forward_refs()
+CredentialCreationCredentialAwsAthenaCredential.update_forward_refs()
+CredentialCreationCredentialAwsAthenaCredentialConfig.update_forward_refs()
 CredentialCreationCredentialAwsRedshiftCredential.update_forward_refs()
 CredentialCreationCredentialAwsRedshiftCredentialConfig.update_forward_refs()
 CredentialCreationCredentialPostgreSqlCredential.update_forward_refs()
 CredentialCreationCredentialPostgreSqlCredentialConfig.update_forward_refs()
 CredentialCreationCredentialSnowflakeCredential.update_forward_refs()
 CredentialCreationCredentialSnowflakeCredentialConfig.update_forward_refs()
+CredentialCreationCredentialKafkaSSLCredential.update_forward_refs()
+CredentialCreationCredentialKafkaSSLCredentialConfig.update_forward_refs()
+CredentialCreationCredentialKafkaSASLPlainCredential.update_forward_refs()
+CredentialCreationCredentialKafkaSASLPlainCredentialConfig.update_forward_refs()
 CredentialSecretChanged.update_forward_refs()
 CredentialSecretChangedErrors.update_forward_refs()
 CredentialUpdate.update_forward_refs()
 CredentialUpdateErrors.update_forward_refs()
 CredentialUpdateCredentialCredential.update_forward_refs()
 CredentialUpdateCredentialAwsCredential.update_forward_refs()
 CredentialUpdateCredentialAwsCredentialConfig.update_forward_refs()
+CredentialUpdateCredentialAwsAthenaCredential.update_forward_refs()
+CredentialUpdateCredentialAwsAthenaCredentialConfig.update_forward_refs()
 CredentialUpdateCredentialAwsRedshiftCredential.update_forward_refs()
 CredentialUpdateCredentialAwsRedshiftCredentialConfig.update_forward_refs()
 CredentialUpdateCredentialPostgreSqlCredential.update_forward_refs()
 CredentialUpdateCredentialPostgreSqlCredentialConfig.update_forward_refs()
 CredentialUpdateCredentialSnowflakeCredential.update_forward_refs()
 CredentialUpdateCredentialSnowflakeCredentialConfig.update_forward_refs()
+CredentialUpdateCredentialKafkaSSLCredential.update_forward_refs()
+CredentialUpdateCredentialKafkaSSLCredentialConfig.update_forward_refs()
+CredentialUpdateCredentialKafkaSASLPlainCredential.update_forward_refs()
+CredentialUpdateCredentialKafkaSASLPlainCredentialConfig.update_forward_refs()
 DestinationCreation.update_forward_refs()
 DestinationCreationErrors.update_forward_refs()
 DestinationCreationDestinationDestination.update_forward_refs()
 DestinationCreationDestinationDestinationCredential.update_forward_refs()
 DestinationCreationDestinationGcpBigQueryDestination.update_forward_refs()
 DestinationCreationDestinationGcpBigQueryDestinationCredential.update_forward_refs()
 DestinationCreationDestinationGcpBigQueryDestinationConfig.update_forward_refs()
@@ -4084,14 +4398,16 @@
 IdentityProviderDeletion.update_forward_refs()
 IdentityProviderDeletionErrors.update_forward_refs()
 IdentityProviderUpdate.update_forward_refs()
 IdentityProviderUpdateErrors.update_forward_refs()
 IdentityProviderUpdateIdentityProviderIdentityProvider.update_forward_refs()
 IdentityProviderUpdateIdentityProviderSamlIdentityProvider.update_forward_refs()
 IdentityProviderUpdateIdentityProviderSamlIdentityProviderConfig.update_forward_refs()
+NamespaceUpdate.update_forward_refs()
+NamespaceUpdateErrors.update_forward_refs()
 NotificationRuleDetails.update_forward_refs()
 NotificationRuleDetailsChannelChannel.update_forward_refs()
 NotificationRuleDetailsChannelSlackChannel.update_forward_refs()
 NotificationRuleDetailsChannelSlackChannelConfig.update_forward_refs()
 NotificationRuleDetailsChannelWebhookChannel.update_forward_refs()
 NotificationRuleDetailsChannelWebhookChannelConfig.update_forward_refs()
 NotificationRuleCreation.update_forward_refs()
@@ -4137,14 +4453,19 @@
 SourceCreationSourceGcpPubSubSourceSegmentations.update_forward_refs()
 SourceCreationSourceGcpPubSubSourceConfig.update_forward_refs()
 SourceCreationSourceGcpPubSubLiteSource.update_forward_refs()
 SourceCreationSourceGcpPubSubLiteSourceCredential.update_forward_refs()
 SourceCreationSourceGcpPubSubLiteSourceWindows.update_forward_refs()
 SourceCreationSourceGcpPubSubLiteSourceSegmentations.update_forward_refs()
 SourceCreationSourceGcpPubSubLiteSourceConfig.update_forward_refs()
+SourceCreationSourceAwsAthenaSource.update_forward_refs()
+SourceCreationSourceAwsAthenaSourceCredential.update_forward_refs()
+SourceCreationSourceAwsAthenaSourceWindows.update_forward_refs()
+SourceCreationSourceAwsAthenaSourceSegmentations.update_forward_refs()
+SourceCreationSourceAwsAthenaSourceConfig.update_forward_refs()
 SourceCreationSourceAwsKinesisSource.update_forward_refs()
 SourceCreationSourceAwsKinesisSourceCredential.update_forward_refs()
 SourceCreationSourceAwsKinesisSourceWindows.update_forward_refs()
 SourceCreationSourceAwsKinesisSourceSegmentations.update_forward_refs()
 SourceCreationSourceAwsKinesisSourceConfig.update_forward_refs()
 SourceCreationSourceAwsRedshiftSource.update_forward_refs()
 SourceCreationSourceAwsRedshiftSourceCredential.update_forward_refs()
@@ -4163,14 +4484,19 @@
 SourceCreationSourcePostgreSqlSourceSegmentations.update_forward_refs()
 SourceCreationSourcePostgreSqlSourceConfig.update_forward_refs()
 SourceCreationSourceSnowflakeSource.update_forward_refs()
 SourceCreationSourceSnowflakeSourceCredential.update_forward_refs()
 SourceCreationSourceSnowflakeSourceWindows.update_forward_refs()
 SourceCreationSourceSnowflakeSourceSegmentations.update_forward_refs()
 SourceCreationSourceSnowflakeSourceConfig.update_forward_refs()
+SourceCreationSourceKafkaSource.update_forward_refs()
+SourceCreationSourceKafkaSourceCredential.update_forward_refs()
+SourceCreationSourceKafkaSourceWindows.update_forward_refs()
+SourceCreationSourceKafkaSourceSegmentations.update_forward_refs()
+SourceCreationSourceKafkaSourceConfig.update_forward_refs()
 SourceUpdate.update_forward_refs()
 SourceUpdateErrors.update_forward_refs()
 SourceUpdateSourceSource.update_forward_refs()
 SourceUpdateSourceSourceCredential.update_forward_refs()
 SourceUpdateSourceSourceWindows.update_forward_refs()
 SourceUpdateSourceSourceSegmentations.update_forward_refs()
 SourceUpdateSourceGcpStorageSource.update_forward_refs()
@@ -4190,14 +4516,19 @@
 SourceUpdateSourceGcpPubSubSourceSegmentations.update_forward_refs()
 SourceUpdateSourceGcpPubSubSourceConfig.update_forward_refs()
 SourceUpdateSourceGcpPubSubLiteSource.update_forward_refs()
 SourceUpdateSourceGcpPubSubLiteSourceCredential.update_forward_refs()
 SourceUpdateSourceGcpPubSubLiteSourceWindows.update_forward_refs()
 SourceUpdateSourceGcpPubSubLiteSourceSegmentations.update_forward_refs()
 SourceUpdateSourceGcpPubSubLiteSourceConfig.update_forward_refs()
+SourceUpdateSourceAwsAthenaSource.update_forward_refs()
+SourceUpdateSourceAwsAthenaSourceCredential.update_forward_refs()
+SourceUpdateSourceAwsAthenaSourceWindows.update_forward_refs()
+SourceUpdateSourceAwsAthenaSourceSegmentations.update_forward_refs()
+SourceUpdateSourceAwsAthenaSourceConfig.update_forward_refs()
 SourceUpdateSourceAwsKinesisSource.update_forward_refs()
 SourceUpdateSourceAwsKinesisSourceCredential.update_forward_refs()
 SourceUpdateSourceAwsKinesisSourceWindows.update_forward_refs()
 SourceUpdateSourceAwsKinesisSourceSegmentations.update_forward_refs()
 SourceUpdateSourceAwsKinesisSourceConfig.update_forward_refs()
 SourceUpdateSourceAwsRedshiftSource.update_forward_refs()
 SourceUpdateSourceAwsRedshiftSourceCredential.update_forward_refs()
@@ -4216,14 +4547,19 @@
 SourceUpdateSourcePostgreSqlSourceSegmentations.update_forward_refs()
 SourceUpdateSourcePostgreSqlSourceConfig.update_forward_refs()
 SourceUpdateSourceSnowflakeSource.update_forward_refs()
 SourceUpdateSourceSnowflakeSourceCredential.update_forward_refs()
 SourceUpdateSourceSnowflakeSourceWindows.update_forward_refs()
 SourceUpdateSourceSnowflakeSourceSegmentations.update_forward_refs()
 SourceUpdateSourceSnowflakeSourceConfig.update_forward_refs()
+SourceUpdateSourceKafkaSource.update_forward_refs()
+SourceUpdateSourceKafkaSourceCredential.update_forward_refs()
+SourceUpdateSourceKafkaSourceWindows.update_forward_refs()
+SourceUpdateSourceKafkaSourceSegmentations.update_forward_refs()
+SourceUpdateSourceKafkaSourceConfig.update_forward_refs()
 UserDetails.update_forward_refs()
 UserDetailsIdentitiesFederatedIdentity.update_forward_refs()
 UserDetailsIdentitiesFederatedIdentityIdp.update_forward_refs()
 UserDetailsIdentitiesLocalIdentity.update_forward_refs()
 UserCreation.update_forward_refs()
 UserCreationErrors.update_forward_refs()
 UserCreationUser.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/gcp_credential_secret_changed.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/gcp_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_channel_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_channel_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_channels.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_credential_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_credential_by_resource_name.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from datetime import datetime
-from typing import Annotated, Literal, Optional, Union
+from typing import Annotated, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from validio_sdk.scalars import CredentialId
 
 from .base_model import BaseModel
 
 
 class GetCredentialByResourceName(BaseModel):
     credential_by_resource_name: Optional[
         Annotated[
             Union[
                 "GetCredentialByResourceNameCredentialByResourceNameCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameAwsCredential",
+                "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential",
                 "GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential",
                 "GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential",
+                "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential",
+                "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="credentialByResourceName")
 
 
 class GetCredentialByResourceNameCredentialByResourceNameCredential(BaseModel):
@@ -46,14 +49,33 @@
     config: "GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig"
 
 
 class GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig(BaseModel):
     access_key: str = Field(alias="accessKey")
 
 
+class GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential(BaseModel):
+    typename__: Literal["AwsAthenaCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig"
+
+
+class GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig(
+    BaseModel
+):
+    access_key: str = Field(alias="accessKey")
+    region: str
+    query_result_location: str = Field(alias="queryResultLocation")
+
+
 class GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential(
     BaseModel
 ):
     typename__: Literal["AwsRedshiftCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
@@ -108,17 +130,64 @@
 class GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig(
     BaseModel
 ):
     account: str
     user: str
 
 
+class GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential(BaseModel):
+    typename__: Literal["KafkaSSLCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig"
+
+
+class GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig(
+    BaseModel
+):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    ca_certificate: str = Field(alias="caCertificate")
+    certificate: str
+    key_password: str = Field(alias="keyPassword")
+
+
+class GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential(
+    BaseModel
+):
+    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig"
+
+
+class GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig(
+    BaseModel
+):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    username: str
+    password: str
+
+
 GetCredentialByResourceName.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameAwsCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameAwsCredentialConfig.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredential.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameAwsAthenaCredentialConfig.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameAwsRedshiftCredentialConfig.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNamePostgreSqlCredentialConfig.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredential.update_forward_refs()
 GetCredentialByResourceNameCredentialByResourceNameSnowflakeCredentialConfig.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredential.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameKafkaSSLCredentialConfig.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredential.update_forward_refs()
+GetCredentialByResourceNameCredentialByResourceNameKafkaSASLPlainCredentialConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_destination_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_destination_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_provider_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_identity_providers.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_identity_providers.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_incidents.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_notification_rule_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_segmentation_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_segmentation_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_source.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,21 @@
         Annotated[
             Union[
                 "GetSourceSourceSource",
                 "GetSourceSourceGcpStorageSource",
                 "GetSourceSourceGcpBigQuerySource",
                 "GetSourceSourceGcpPubSubSource",
                 "GetSourceSourceGcpPubSubLiteSource",
+                "GetSourceSourceAwsAthenaSource",
                 "GetSourceSourceAwsKinesisSource",
                 "GetSourceSourceAwsRedshiftSource",
                 "GetSourceSourceAwsS3Source",
                 "GetSourceSourcePostgreSqlSource",
                 "GetSourceSourceSnowflakeSource",
+                "GetSourceSourceKafkaSource",
             ],
             Field(discriminator="typename__"),
         ]
     ]
 
 
 class GetSourceSourceSource(BaseModel):
@@ -255,14 +257,61 @@
 
 class GetSourceSourceGcpPubSubLiteSourceConfig(BaseModel):
     location: str
     project: str
     subscription_id: str = Field(alias="subscriptionId")
 
 
+class GetSourceSourceAwsAthenaSource(BaseModel):
+    typename__: Literal["AwsAthenaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "GetSourceSourceAwsAthenaSourceCredential"
+    windows: List["GetSourceSourceAwsAthenaSourceWindows"]
+    segmentations: List["GetSourceSourceAwsAthenaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetSourceSourceAwsAthenaSourceConfig"
+
+
+class GetSourceSourceAwsAthenaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceSourceAwsAthenaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceSourceAwsAthenaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceSourceAwsAthenaSourceConfig(BaseModel):
+    catalog: str
+    database: str
+    table: str
+    cursor_field: str = Field(alias="cursorField")
+    lookback_days: int = Field(alias="lookbackDays")
+    schedule: CronExpression
+
+
 class GetSourceSourceAwsKinesisSource(BaseModel):
     typename__: Literal["AwsKinesisSource"] = Field(alias="__typename")
     id: SourceId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     credential: "GetSourceSourceAwsKinesisSourceCredential"
@@ -492,14 +541,56 @@
     db_schema: Any = Field(alias="schema")
     table: str
     cursor_field: str = Field(alias="cursorField")
     lookback_days: int = Field(alias="lookbackDays")
     schedule: CronExpression
 
 
+class GetSourceSourceKafkaSource(BaseModel):
+    typename__: Literal["KafkaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "GetSourceSourceKafkaSourceCredential"
+    windows: List["GetSourceSourceKafkaSourceWindows"]
+    segmentations: List["GetSourceSourceKafkaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetSourceSourceKafkaSourceConfig"
+
+
+class GetSourceSourceKafkaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceSourceKafkaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceSourceKafkaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceSourceKafkaSourceConfig(BaseModel):
+    topic: str
+
+
 GetSource.update_forward_refs()
 GetSourceSourceSource.update_forward_refs()
 GetSourceSourceSourceCredential.update_forward_refs()
 GetSourceSourceSourceWindows.update_forward_refs()
 GetSourceSourceSourceSegmentations.update_forward_refs()
 GetSourceSourceGcpStorageSource.update_forward_refs()
 GetSourceSourceGcpStorageSourceCredential.update_forward_refs()
@@ -518,14 +609,19 @@
 GetSourceSourceGcpPubSubSourceSegmentations.update_forward_refs()
 GetSourceSourceGcpPubSubSourceConfig.update_forward_refs()
 GetSourceSourceGcpPubSubLiteSource.update_forward_refs()
 GetSourceSourceGcpPubSubLiteSourceCredential.update_forward_refs()
 GetSourceSourceGcpPubSubLiteSourceWindows.update_forward_refs()
 GetSourceSourceGcpPubSubLiteSourceSegmentations.update_forward_refs()
 GetSourceSourceGcpPubSubLiteSourceConfig.update_forward_refs()
+GetSourceSourceAwsAthenaSource.update_forward_refs()
+GetSourceSourceAwsAthenaSourceCredential.update_forward_refs()
+GetSourceSourceAwsAthenaSourceWindows.update_forward_refs()
+GetSourceSourceAwsAthenaSourceSegmentations.update_forward_refs()
+GetSourceSourceAwsAthenaSourceConfig.update_forward_refs()
 GetSourceSourceAwsKinesisSource.update_forward_refs()
 GetSourceSourceAwsKinesisSourceCredential.update_forward_refs()
 GetSourceSourceAwsKinesisSourceWindows.update_forward_refs()
 GetSourceSourceAwsKinesisSourceSegmentations.update_forward_refs()
 GetSourceSourceAwsKinesisSourceConfig.update_forward_refs()
 GetSourceSourceAwsRedshiftSource.update_forward_refs()
 GetSourceSourceAwsRedshiftSourceCredential.update_forward_refs()
@@ -544,7 +640,12 @@
 GetSourceSourcePostgreSqlSourceSegmentations.update_forward_refs()
 GetSourceSourcePostgreSqlSourceConfig.update_forward_refs()
 GetSourceSourceSnowflakeSource.update_forward_refs()
 GetSourceSourceSnowflakeSourceCredential.update_forward_refs()
 GetSourceSourceSnowflakeSourceWindows.update_forward_refs()
 GetSourceSourceSnowflakeSourceSegmentations.update_forward_refs()
 GetSourceSourceSnowflakeSourceConfig.update_forward_refs()
+GetSourceSourceKafkaSource.update_forward_refs()
+GetSourceSourceKafkaSourceCredential.update_forward_refs()
+GetSourceSourceKafkaSourceWindows.update_forward_refs()
+GetSourceSourceKafkaSourceSegmentations.update_forward_refs()
+GetSourceSourceKafkaSourceConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_source_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_by_resource_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,21 @@
         Annotated[
             Union[
                 "GetSourceByResourceNameSourceByResourceNameSource",
                 "GetSourceByResourceNameSourceByResourceNameGcpStorageSource",
                 "GetSourceByResourceNameSourceByResourceNameGcpBigQuerySource",
                 "GetSourceByResourceNameSourceByResourceNameGcpPubSubSource",
                 "GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSource",
+                "GetSourceByResourceNameSourceByResourceNameAwsAthenaSource",
                 "GetSourceByResourceNameSourceByResourceNameAwsKinesisSource",
                 "GetSourceByResourceNameSourceByResourceNameAwsRedshiftSource",
                 "GetSourceByResourceNameSourceByResourceNameAwsS3Source",
                 "GetSourceByResourceNameSourceByResourceNamePostgreSqlSource",
                 "GetSourceByResourceNameSourceByResourceNameSnowflakeSource",
+                "GetSourceByResourceNameSourceByResourceNameKafkaSource",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="sourceByResourceName")
 
 
 class GetSourceByResourceNameSourceByResourceNameSource(BaseModel):
@@ -277,14 +279,65 @@
 
 class GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSourceConfig(BaseModel):
     location: str
     project: str
     subscription_id: str = Field(alias="subscriptionId")
 
 
+class GetSourceByResourceNameSourceByResourceNameAwsAthenaSource(BaseModel):
+    typename__: Literal["AwsAthenaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceCredential"
+    windows: List["GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceWindows"]
+    segmentations: List[
+        "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceSegmentations"
+    ]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceConfig"
+
+
+class GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceSegmentations(
+    BaseModel
+):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceConfig(BaseModel):
+    catalog: str
+    database: str
+    table: str
+    cursor_field: str = Field(alias="cursorField")
+    lookback_days: int = Field(alias="lookbackDays")
+    schedule: CronExpression
+
+
 class GetSourceByResourceNameSourceByResourceNameAwsKinesisSource(BaseModel):
     typename__: Literal["AwsKinesisSource"] = Field(alias="__typename")
     id: SourceId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     credential: "GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceCredential"
@@ -532,14 +585,58 @@
     db_schema: Any = Field(alias="schema")
     table: str
     cursor_field: str = Field(alias="cursorField")
     lookback_days: int = Field(alias="lookbackDays")
     schedule: CronExpression
 
 
+class GetSourceByResourceNameSourceByResourceNameKafkaSource(BaseModel):
+    typename__: Literal["KafkaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "GetSourceByResourceNameSourceByResourceNameKafkaSourceCredential"
+    windows: List["GetSourceByResourceNameSourceByResourceNameKafkaSourceWindows"]
+    segmentations: List[
+        "GetSourceByResourceNameSourceByResourceNameKafkaSourceSegmentations"
+    ]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "GetSourceByResourceNameSourceByResourceNameKafkaSourceConfig"
+
+
+class GetSourceByResourceNameSourceByResourceNameKafkaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceByResourceNameSourceByResourceNameKafkaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceByResourceNameSourceByResourceNameKafkaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class GetSourceByResourceNameSourceByResourceNameKafkaSourceConfig(BaseModel):
+    topic: str
+
+
 GetSourceByResourceName.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSource.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSourceCredential.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSourceWindows.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSourceSegmentations.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpStorageSource.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpStorageSourceCredential.update_forward_refs()
@@ -558,14 +655,19 @@
 GetSourceByResourceNameSourceByResourceNameGcpPubSubSourceSegmentations.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpPubSubSourceConfig.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSource.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSourceCredential.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSourceWindows.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSourceSegmentations.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameGcpPubSubLiteSourceConfig.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameAwsAthenaSource.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceCredential.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceWindows.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceSegmentations.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameAwsAthenaSourceConfig.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsKinesisSource.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceCredential.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceWindows.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceSegmentations.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsKinesisSourceConfig.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsRedshiftSource.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameAwsRedshiftSourceCredential.update_forward_refs()
@@ -584,7 +686,12 @@
 GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceSegmentations.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNamePostgreSqlSourceConfig.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSnowflakeSource.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSnowflakeSourceCredential.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSnowflakeSourceWindows.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSnowflakeSourceSegmentations.update_forward_refs()
 GetSourceByResourceNameSourceByResourceNameSnowflakeSourceConfig.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameKafkaSource.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameKafkaSourceCredential.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameKafkaSourceWindows.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameKafkaSourceSegmentations.update_forward_refs()
+GetSourceByResourceNameSourceByResourceNameKafkaSourceConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_source_incidents.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_source_recommended_validators.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_source_recommended_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,28 +48,36 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
 
 
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorProgress(
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSegmentation"
 
 
@@ -94,14 +102,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorConfig"
 
 
@@ -109,14 +118,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSegmentation"
 
 
@@ -147,14 +163,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorConfig"
 
 
@@ -162,14 +179,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSegmentation"
 
 
@@ -202,14 +226,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorConfig"
 
 
@@ -217,14 +242,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSegmentation"
 
 
@@ -255,14 +287,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorConfig"
 
 
@@ -270,14 +303,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSegmentation"
 
 
@@ -308,14 +348,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorConfig"
 
 
@@ -323,14 +364,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSegmentation"
 
 
@@ -361,14 +409,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorConfig"
 
 
@@ -376,14 +425,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSegmentation"
 
 
@@ -414,14 +470,15 @@
     has_custom_name: bool = Field(alias="hasCustomName")
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     state: ValidatorState
     progress: Optional[
         "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorProgress"
     ]
+    stats: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorStats"
     state_updated_at: datetime = Field(alias="stateUpdatedAt")
     source_config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfig" = Field(
         alias="sourceConfig"
     )
     config: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorConfig"
 
 
@@ -429,14 +486,21 @@
     BaseModel
 ):
     percentage: float
     processed: int
     total: int
 
 
+class GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorStats(
+    BaseModel
+):
+    last_artifact_at: Optional[datetime] = Field(alias="lastArtifactAt")
+    last_incident_at: Optional[datetime] = Field(alias="lastIncidentAt")
+
+
 class GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfig(
     BaseModel
 ):
     source: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSource"
     segmentation: "GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSegmentation"
 
 
@@ -458,52 +522,60 @@
     relative_volume_metric: RelativeVolumeMetric = Field(alias="relativeVolumeMetric")
 
 
 GetSourceRecommendedValidators.update_forward_refs()
 GetSourceRecommendedValidatorsSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericValidatorConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsCategoricalDistributionValidatorConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericDistributionValidatorConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsVolumeValidatorConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsNumericAnomalyValidatorConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeTimeValidatorConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidator.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorProgress.update_forward_refs()
+GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorStats.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfig.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSource.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorSourceConfigSegmentation.update_forward_refs()
 GetSourceRecommendedValidatorsSourceRecommendedValidatorsRelativeVolumeValidatorConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_segment_incidents.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_incidents.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_validator_segment_metrics.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_validator_segment_metrics.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/get_window_by_resource_name.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/get_window_by_resource_name.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/input_types.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/input_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,60 @@
     Role,
     UserStatus,
     VolumeMetric,
     WindowTimeUnit,
 )
 
 
+class AwsAthenaCredentialCreateInput(BaseModel):
+    access_key: str = Field(alias="accessKey")
+    name: str
+    query_result_location: str = Field(alias="queryResultLocation")
+    region: str
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+    secret_key: str = Field(alias="secretKey")
+
+
+class AwsAthenaCredentialUpdateInput(BaseModel):
+    access_key: str = Field(alias="accessKey")
+    id: CredentialId
+    query_result_location: str = Field(alias="queryResultLocation")
+    region: str
+    secret_key: str = Field(alias="secretKey")
+
+
+class AwsAthenaInferSchemaInput(BaseModel):
+    catalog: str
+    credential_id: CredentialId = Field(alias="credentialId")
+    database: str
+    table: str
+
+
+class AwsAthenaSourceCreateInput(BaseModel):
+    catalog: str
+    credential_id: CredentialId = Field(alias="credentialId")
+    cursor_field: str = Field(alias="cursorField")
+    database: str
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    lookback_days: int = Field(alias="lookbackDays")
+    name: str
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+    schedule: CronExpression
+    table: str
+
+
+class AwsAthenaSourceUpdateInput(BaseModel):
+    id: SourceId
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    lookback_days: int = Field(alias="lookbackDays")
+    schedule: CronExpression
+
+
 class AwsCredentialCreateInput(BaseModel):
     access_key: str = Field(alias="accessKey")
     name: str
     resource_name: Optional[str] = Field(alias="resourceName")
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
     secret_key: str = Field(alias="secretKey")
 
@@ -414,14 +460,82 @@
     id: str
 
 
 class IncidentsInput(BaseModel):
     time_range: "TimeRangeInput" = Field(alias="timeRange")
 
 
+class KafkaInferSchemaInput(BaseModel):
+    credential_id: CredentialId = Field(alias="credentialId")
+    topic: str
+
+
+class KafkaSASLPlainCredentialCreateInput(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    name: str
+    password: str
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+    username: str
+
+
+class KafkaSASLPlainCredentialSecretChangedInput(BaseModel):
+    id: CredentialId
+    password: str
+
+
+class KafkaSASLPlainCredentialUpdateInput(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    id: CredentialId
+    password: str
+    username: str
+
+
+class KafkaSSLCredentialCreateInput(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    ca_certificate: str = Field(alias="caCertificate")
+    client_certificate: str = Field(alias="clientCertificate")
+    client_private_key: str = Field(alias="clientPrivateKey")
+    client_private_key_password: str = Field(alias="clientPrivateKeyPassword")
+    name: str
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+
+
+class KafkaSSLCredentialSecretChangedInput(BaseModel):
+    ca_certificate: str = Field(alias="caCertificate")
+    client_certificate: str = Field(alias="clientCertificate")
+    client_private_key: str = Field(alias="clientPrivateKey")
+    client_private_key_password: str = Field(alias="clientPrivateKeyPassword")
+    id: CredentialId
+
+
+class KafkaSSLCredentialUpdateInput(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    ca_certificate: str = Field(alias="caCertificate")
+    client_certificate: str = Field(alias="clientCertificate")
+    client_private_key: str = Field(alias="clientPrivateKey")
+    client_private_key_password: str = Field(alias="clientPrivateKeyPassword")
+    id: CredentialId
+
+
+class KafkaSourceCreateInput(BaseModel):
+    credential_id: CredentialId = Field(alias="credentialId")
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    name: str
+    resource_name: Optional[str] = Field(alias="resourceName")
+    resource_namespace: Optional[str] = Field(alias="resourceNamespace")
+    topic: str
+
+
+class KafkaSourceUpdateInput(BaseModel):
+    id: SourceId
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+
+
 class LocalIdentityProviderUpdateInput(BaseModel):
     disabled: bool
     id: str
     name: str
 
 
 class MonotonicThresholdCreateInput(BaseModel):
@@ -625,14 +739,20 @@
     source_config: "SourceConfigUpdateInput" = Field(alias="sourceConfig")
 
 
 class ResourceFilter(BaseModel):
     resource_namespace: Optional[str] = Field(alias="resourceNamespace")
 
 
+class ResourceNamespaceUpdateInput(BaseModel):
+    new_resource_namespace: str = Field(alias="newResourceNamespace")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
 class SamlIdentityProviderCreateInput(BaseModel):
     cert: str
     disabled: bool
     entity_id: str = Field(alias="entityId")
     entry_point: str = Field(alias="entryPoint")
     name: str
     resource_name: Optional[str] = Field(alias="resourceName")
@@ -905,14 +1025,19 @@
     application_link_url: str = Field(alias="applicationLinkUrl")
     auth_header: Optional[str] = Field(alias="authHeader")
     id: Any
     name: Optional[str]
     webhook_url: str = Field(alias="webhookUrl")
 
 
+AwsAthenaCredentialCreateInput.update_forward_refs()
+AwsAthenaCredentialUpdateInput.update_forward_refs()
+AwsAthenaInferSchemaInput.update_forward_refs()
+AwsAthenaSourceCreateInput.update_forward_refs()
+AwsAthenaSourceUpdateInput.update_forward_refs()
 AwsCredentialCreateInput.update_forward_refs()
 AwsCredentialSecretChangedInput.update_forward_refs()
 AwsCredentialUpdateInput.update_forward_refs()
 AwsKinesisDestinationCreateInput.update_forward_refs()
 AwsKinesisDestinationUpdateInput.update_forward_refs()
 AwsKinesisInferSchemaInput.update_forward_refs()
 AwsKinesisSourceCreateInput.update_forward_refs()
@@ -955,14 +1080,23 @@
 GcpPubSubSourceUpdateInput.update_forward_refs()
 GcpStorageInferSchemaInput.update_forward_refs()
 GcpStorageSourceCreateInput.update_forward_refs()
 GcpStorageSourceUpdateInput.update_forward_refs()
 IdentityDeleteInput.update_forward_refs()
 IdentityProviderDeleteInput.update_forward_refs()
 IncidentsInput.update_forward_refs()
+KafkaInferSchemaInput.update_forward_refs()
+KafkaSASLPlainCredentialCreateInput.update_forward_refs()
+KafkaSASLPlainCredentialSecretChangedInput.update_forward_refs()
+KafkaSASLPlainCredentialUpdateInput.update_forward_refs()
+KafkaSSLCredentialCreateInput.update_forward_refs()
+KafkaSSLCredentialSecretChangedInput.update_forward_refs()
+KafkaSSLCredentialUpdateInput.update_forward_refs()
+KafkaSourceCreateInput.update_forward_refs()
+KafkaSourceUpdateInput.update_forward_refs()
 LocalIdentityProviderUpdateInput.update_forward_refs()
 MonotonicThresholdCreateInput.update_forward_refs()
 NotificationRuleCreateInput.update_forward_refs()
 NotificationRuleDeleteInput.update_forward_refs()
 NotificationRuleUpdateInput.update_forward_refs()
 NumericAnomalyValidatorCreateInput.update_forward_refs()
 NumericAnomalyValidatorUpdateInput.update_forward_refs()
@@ -979,14 +1113,15 @@
 ReferenceSourceConfigCreateInput.update_forward_refs()
 ReferenceSourceConfigUpdateInput.update_forward_refs()
 RelativeTimeValidatorCreateInput.update_forward_refs()
 RelativeTimeValidatorUpdateInput.update_forward_refs()
 RelativeVolumeValidatorCreateInput.update_forward_refs()
 RelativeVolumeValidatorUpdateInput.update_forward_refs()
 ResourceFilter.update_forward_refs()
+ResourceNamespaceUpdateInput.update_forward_refs()
 SamlIdentityProviderCreateInput.update_forward_refs()
 SamlIdentityProviderUpdateInput.update_forward_refs()
 SegmentIncidentsInput.update_forward_refs()
 SegmentationCreateInput.update_forward_refs()
 SessionizedWindowCreateInput.update_forward_refs()
 SessionizedWindowUpdateInput.update_forward_refs()
 SlackChannelCreateInput.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/list_credentials.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/list_credentials.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 
 class ListCredentials(BaseModel):
     credentials_list: List[
         Annotated[
             Union[
                 "ListCredentialsCredentialsListCredential",
                 "ListCredentialsCredentialsListAwsCredential",
+                "ListCredentialsCredentialsListAwsAthenaCredential",
                 "ListCredentialsCredentialsListAwsRedshiftCredential",
                 "ListCredentialsCredentialsListPostgreSqlCredential",
                 "ListCredentialsCredentialsListSnowflakeCredential",
+                "ListCredentialsCredentialsListKafkaSSLCredential",
+                "ListCredentialsCredentialsListKafkaSASLPlainCredential",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="credentialsList")
 
 
 class ListCredentialsCredentialsListCredential(BaseModel):
@@ -46,14 +49,31 @@
     config: "ListCredentialsCredentialsListAwsCredentialConfig"
 
 
 class ListCredentialsCredentialsListAwsCredentialConfig(BaseModel):
     access_key: str = Field(alias="accessKey")
 
 
+class ListCredentialsCredentialsListAwsAthenaCredential(BaseModel):
+    typename__: Literal["AwsAthenaCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "ListCredentialsCredentialsListAwsAthenaCredentialConfig"
+
+
+class ListCredentialsCredentialsListAwsAthenaCredentialConfig(BaseModel):
+    access_key: str = Field(alias="accessKey")
+    region: str
+    query_result_location: str = Field(alias="queryResultLocation")
+
+
 class ListCredentialsCredentialsListAwsRedshiftCredential(BaseModel):
     typename__: Literal["AwsRedshiftCredential"] = Field(alias="__typename")
     id: CredentialId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     resource_name: str = Field(alias="resourceName")
@@ -98,17 +118,58 @@
 
 
 class ListCredentialsCredentialsListSnowflakeCredentialConfig(BaseModel):
     account: str
     user: str
 
 
+class ListCredentialsCredentialsListKafkaSSLCredential(BaseModel):
+    typename__: Literal["KafkaSSLCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "ListCredentialsCredentialsListKafkaSSLCredentialConfig"
+
+
+class ListCredentialsCredentialsListKafkaSSLCredentialConfig(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    ca_certificate: str = Field(alias="caCertificate")
+    certificate: str
+    key_password: str = Field(alias="keyPassword")
+
+
+class ListCredentialsCredentialsListKafkaSASLPlainCredential(BaseModel):
+    typename__: Literal["KafkaSASLPlainCredential"] = Field(alias="__typename")
+    id: CredentialId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig"
+
+
+class ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig(BaseModel):
+    bootstrap_servers: List[str] = Field(alias="bootstrapServers")
+    username: str
+    password: str
+
+
 ListCredentials.update_forward_refs()
 ListCredentialsCredentialsListCredential.update_forward_refs()
 ListCredentialsCredentialsListAwsCredential.update_forward_refs()
 ListCredentialsCredentialsListAwsCredentialConfig.update_forward_refs()
+ListCredentialsCredentialsListAwsAthenaCredential.update_forward_refs()
+ListCredentialsCredentialsListAwsAthenaCredentialConfig.update_forward_refs()
 ListCredentialsCredentialsListAwsRedshiftCredential.update_forward_refs()
 ListCredentialsCredentialsListAwsRedshiftCredentialConfig.update_forward_refs()
 ListCredentialsCredentialsListPostgreSqlCredential.update_forward_refs()
 ListCredentialsCredentialsListPostgreSqlCredentialConfig.update_forward_refs()
 ListCredentialsCredentialsListSnowflakeCredential.update_forward_refs()
 ListCredentialsCredentialsListSnowflakeCredentialConfig.update_forward_refs()
+ListCredentialsCredentialsListKafkaSSLCredential.update_forward_refs()
+ListCredentialsCredentialsListKafkaSSLCredentialConfig.update_forward_refs()
+ListCredentialsCredentialsListKafkaSASLPlainCredential.update_forward_refs()
+ListCredentialsCredentialsListKafkaSASLPlainCredentialConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/list_destinations.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/list_destinations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/list_sources.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/list_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,21 @@
         Annotated[
             Union[
                 "ListSourcesSourcesListSource",
                 "ListSourcesSourcesListGcpStorageSource",
                 "ListSourcesSourcesListGcpBigQuerySource",
                 "ListSourcesSourcesListGcpPubSubSource",
                 "ListSourcesSourcesListGcpPubSubLiteSource",
+                "ListSourcesSourcesListAwsAthenaSource",
                 "ListSourcesSourcesListAwsKinesisSource",
                 "ListSourcesSourcesListAwsRedshiftSource",
                 "ListSourcesSourcesListAwsS3Source",
                 "ListSourcesSourcesListPostgreSqlSource",
                 "ListSourcesSourcesListSnowflakeSource",
+                "ListSourcesSourcesListKafkaSource",
             ],
             Field(discriminator="typename__"),
         ]
     ] = Field(alias="sourcesList")
 
 
 class ListSourcesSourcesListSource(BaseModel):
@@ -255,14 +257,61 @@
 
 class ListSourcesSourcesListGcpPubSubLiteSourceConfig(BaseModel):
     location: str
     project: str
     subscription_id: str = Field(alias="subscriptionId")
 
 
+class ListSourcesSourcesListAwsAthenaSource(BaseModel):
+    typename__: Literal["AwsAthenaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "ListSourcesSourcesListAwsAthenaSourceCredential"
+    windows: List["ListSourcesSourcesListAwsAthenaSourceWindows"]
+    segmentations: List["ListSourcesSourcesListAwsAthenaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "ListSourcesSourcesListAwsAthenaSourceConfig"
+
+
+class ListSourcesSourcesListAwsAthenaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class ListSourcesSourcesListAwsAthenaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class ListSourcesSourcesListAwsAthenaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class ListSourcesSourcesListAwsAthenaSourceConfig(BaseModel):
+    catalog: str
+    database: str
+    table: str
+    cursor_field: str = Field(alias="cursorField")
+    lookback_days: int = Field(alias="lookbackDays")
+    schedule: CronExpression
+
+
 class ListSourcesSourcesListAwsKinesisSource(BaseModel):
     typename__: Literal["AwsKinesisSource"] = Field(alias="__typename")
     id: SourceId
     name: str
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     credential: "ListSourcesSourcesListAwsKinesisSourceCredential"
@@ -492,14 +541,56 @@
     db_schema: Any = Field(alias="schema")
     table: str
     cursor_field: str = Field(alias="cursorField")
     lookback_days: int = Field(alias="lookbackDays")
     schedule: CronExpression
 
 
+class ListSourcesSourcesListKafkaSource(BaseModel):
+    typename__: Literal["KafkaSource"] = Field(alias="__typename")
+    id: SourceId
+    name: str
+    created_at: datetime = Field(alias="createdAt")
+    updated_at: datetime = Field(alias="updatedAt")
+    credential: "ListSourcesSourcesListKafkaSourceCredential"
+    windows: List["ListSourcesSourcesListKafkaSourceWindows"]
+    segmentations: List["ListSourcesSourcesListKafkaSourceSegmentations"]
+    jtd_schema: JsonTypeDefinition = Field(alias="jtdSchema")
+    state: SourceState
+    state_updated_at: datetime = Field(alias="stateUpdatedAt")
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+    config: "ListSourcesSourcesListKafkaSourceConfig"
+
+
+class ListSourcesSourcesListKafkaSourceCredential(BaseModel):
+    id: CredentialId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class ListSourcesSourcesListKafkaSourceWindows(BaseModel):
+    id: WindowId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class ListSourcesSourcesListKafkaSourceSegmentations(BaseModel):
+    id: SegmentationId
+    name: str
+    resource_name: str = Field(alias="resourceName")
+    resource_namespace: str = Field(alias="resourceNamespace")
+
+
+class ListSourcesSourcesListKafkaSourceConfig(BaseModel):
+    topic: str
+
+
 ListSources.update_forward_refs()
 ListSourcesSourcesListSource.update_forward_refs()
 ListSourcesSourcesListSourceCredential.update_forward_refs()
 ListSourcesSourcesListSourceWindows.update_forward_refs()
 ListSourcesSourcesListSourceSegmentations.update_forward_refs()
 ListSourcesSourcesListGcpStorageSource.update_forward_refs()
 ListSourcesSourcesListGcpStorageSourceCredential.update_forward_refs()
@@ -518,14 +609,19 @@
 ListSourcesSourcesListGcpPubSubSourceSegmentations.update_forward_refs()
 ListSourcesSourcesListGcpPubSubSourceConfig.update_forward_refs()
 ListSourcesSourcesListGcpPubSubLiteSource.update_forward_refs()
 ListSourcesSourcesListGcpPubSubLiteSourceCredential.update_forward_refs()
 ListSourcesSourcesListGcpPubSubLiteSourceWindows.update_forward_refs()
 ListSourcesSourcesListGcpPubSubLiteSourceSegmentations.update_forward_refs()
 ListSourcesSourcesListGcpPubSubLiteSourceConfig.update_forward_refs()
+ListSourcesSourcesListAwsAthenaSource.update_forward_refs()
+ListSourcesSourcesListAwsAthenaSourceCredential.update_forward_refs()
+ListSourcesSourcesListAwsAthenaSourceWindows.update_forward_refs()
+ListSourcesSourcesListAwsAthenaSourceSegmentations.update_forward_refs()
+ListSourcesSourcesListAwsAthenaSourceConfig.update_forward_refs()
 ListSourcesSourcesListAwsKinesisSource.update_forward_refs()
 ListSourcesSourcesListAwsKinesisSourceCredential.update_forward_refs()
 ListSourcesSourcesListAwsKinesisSourceWindows.update_forward_refs()
 ListSourcesSourcesListAwsKinesisSourceSegmentations.update_forward_refs()
 ListSourcesSourcesListAwsKinesisSourceConfig.update_forward_refs()
 ListSourcesSourcesListAwsRedshiftSource.update_forward_refs()
 ListSourcesSourcesListAwsRedshiftSourceCredential.update_forward_refs()
@@ -544,7 +640,12 @@
 ListSourcesSourcesListPostgreSqlSourceSegmentations.update_forward_refs()
 ListSourcesSourcesListPostgreSqlSourceConfig.update_forward_refs()
 ListSourcesSourcesListSnowflakeSource.update_forward_refs()
 ListSourcesSourcesListSnowflakeSourceCredential.update_forward_refs()
 ListSourcesSourcesListSnowflakeSourceWindows.update_forward_refs()
 ListSourcesSourcesListSnowflakeSourceSegmentations.update_forward_refs()
 ListSourcesSourcesListSnowflakeSourceConfig.update_forward_refs()
+ListSourcesSourcesListKafkaSource.update_forward_refs()
+ListSourcesSourcesListKafkaSourceCredential.update_forward_refs()
+ListSourcesSourcesListKafkaSourceWindows.update_forward_refs()
+ListSourcesSourcesListKafkaSourceSegmentations.update_forward_refs()
+ListSourcesSourcesListKafkaSourceConfig.update_forward_refs()
```

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/list_validators.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/list_validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/list_windows.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/list_windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/postgre_sql_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/scalars.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/snowflake_credential_secret_changed.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/snowflake_credential_secret_changed.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/start_source.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/start_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/stop_source.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/stop_source.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_kinesis_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_kinesis_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_aws_redshift_credential.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_aws_redshift_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_categorical_distribution_validator.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_categorical_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_gcp_big_query_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_gcp_big_query_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_local_identity_provider.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_local_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_numeric_anomaly_validator.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_anomaly_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_numeric_distribution_validator.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_numeric_distribution_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_postgre_sql_credential.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_postgre_sql_credential.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_relative_time_validator.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_time_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_relative_volume_validator.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_relative_volume_validator.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_saml_identity_provider.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_saml_identity_provider.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_snowflake_destination.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_snowflake_destination.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_dynamic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_fixed_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py` & `validio_sdk-0.6.0/validio_sdk/graphql_client/update_validator_with_monotonic_threshold.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_diff.py` & `validio_sdk-0.6.0/validio_sdk/resource/_diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_diffable.py` & `validio_sdk-0.6.0/validio_sdk/resource/_diffable.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_errors.py` & `validio_sdk-0.6.0/validio_sdk/resource/_errors.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_field_selector.py` & `validio_sdk-0.6.0/validio_sdk/resource/_field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_resource.py` & `validio_sdk-0.6.0/validio_sdk/resource/_resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_resource_graph.py` & `validio_sdk-0.6.0/validio_sdk/resource/_resource_graph.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_serde.py` & `validio_sdk-0.6.0/validio_sdk/resource/_serde.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_server_resources.py` & `validio_sdk-0.6.0/validio_sdk/resource/_server_resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     DiffContext,
     GraphDiff,
     ResourceUpdates,
     expand_validator_field_selectors,
     infer_schema_for_source,
 )
 from validio_sdk.resource._diff_util import (
+    must_find_channel,
+    must_find_credential,
     must_find_destination,
     must_find_segmentation,
     must_find_source,
     must_find_window,
 )
 from validio_sdk.resource._resource import Resource, ResourceGraph
 from validio_sdk.resource._util import _sanitize_error
@@ -78,14 +80,17 @@
     client: ValidioAPIClient,
     g: ResourceGraph,
     ctx: DiffContext,
 ):
     credentials = await client.list_credentials()
 
     for c in credentials:
+        if c.resource_namespace != namespace:
+            continue
+
         name = c.resource_name
 
         # The 'secret' parts of a credential are left unset since they are not
         # provided by the API. We check for changes to them specially.
         match c.typename__:
             case "DemoCredential":
                 credential: Credential = DemoCredential(name=name, __internal__=g)
@@ -152,14 +157,17 @@
     # We need to import the module due to the `eval`
     # ruff: noqa: F401
     from validio_sdk.resource import channels
 
     server_channels = await client.get_channels()
 
     for ch in server_channels:
+        if ch.resource_namespace != namespace:
+            continue
+
         name = ch.resource_name
 
         cls = eval(f"validio_sdk.resource.channels.{ch.typename__}")
         channel = cls(
             **{
                 **ch.config.__dict__,  # type: ignore
                 "name": name,
@@ -180,27 +188,30 @@
     # ruff: noqa: F401
     from validio_sdk.resource import notification_rules
 
     rules = await client.get_notification_rules()
 
     source_lookup_by_id = {s._must_id(): s for s in ctx.sources.values()}
     for r in rules:
+        if r.resource_namespace != namespace:
+            continue
+
         name = r.resource_name
 
         cls = eval(f"validio_sdk.resource.notification_rules.{r.typename__}")
         fields = list(inspect.signature(cls).parameters)
         rule = cls(
             **{
                 **{
                     f: getattr(r, f)
                     for f in fields
                     if f not in {"name", "channel", "sources"}
                 },
                 "name": name,
-                "channel": ctx.channels[r.channel.resource_name],
+                "channel": must_find_channel(ctx, r.channel.resource_name),
                 "sources": [
                     source_lookup_by_id[sid]
                     for sid in r.sources
                     if sid and sid in source_lookup_by_id
                 ],
             }
         )
@@ -217,22 +228,25 @@
     # We need to import the module due to the `eval`
     # ruff: noqa: F401
     from validio_sdk.resource import destinations
 
     server_destinations = await client.list_destinations()
 
     for d in server_destinations:
+        if d.resource_namespace != namespace:
+            continue
+
         name = d.resource_name
 
         cls = eval(f"validio_sdk.resource.destinations.{d.typename__}")
         destination = cls(
             **{
                 **d.config.__dict__,  # type: ignore
                 "name": name,
-                "credential": ctx.credentials[d.credential.resource_name],
+                "credential": must_find_credential(ctx, d.credential.resource_name),
             }
         )
         destination._id.value = d.id
         destination._namespace = d.resource_namespace
         ctx.destinations[name] = destination
 
 
@@ -244,23 +258,26 @@
     # We need to import the module due to the `eval`
     # ruff: noqa: F401
     from validio_sdk.resource import sources
 
     server_sources = await client.list_sources()
 
     for s in server_sources:
+        if s.resource_namespace != namespace:
+            continue
+
         name = s.resource_name
 
         cls = eval(f"validio_sdk.resource.sources.{s.typename__}")
         params = s.config.__dict__ if hasattr(s, "config") else {}
         source = cls(
             **{
                 **params,
                 "name": name,
-                "credential": ctx.credentials[s.credential.resource_name],
+                "credential": must_find_credential(ctx, s.credential.resource_name),
                 "jtd_schema": s.jtd_schema,
             }
         )
         source._id.value = s.id
         source._namespace = s.resource_namespace
         ctx.sources[name] = source
 
@@ -273,14 +290,17 @@
     # We need to import the module due to the `eval`
     # ruff: noqa: F401
     from validio_sdk.resource import segmentations
 
     server_segmentations = await client.list_segmentations()
 
     for s in server_segmentations:
+        if s.resource_namespace != namespace:
+            continue
+
         name = s.resource_name
 
         segmentation = Segmentation(
             name=name,
             source=must_find_source(ctx, s.source.resource_name),
             fields=s.fields,
         )
@@ -298,14 +318,17 @@
     # We need to import the module due to the `eval`
     # ruff: noqa: F401
     from validio_sdk.resource import windows
 
     server_windows = await client.list_windows()
 
     for w in server_windows:
+        if w.resource_namespace != namespace:
+            continue
+
         name = w.resource_name
 
         cls = None
         for c in WINDOW_CLASSES:
             if w.typename__ == c.__name__:
                 cls = c
                 break
@@ -367,14 +390,17 @@
     client: ValidioAPIClient,
     ctx: DiffContext,
 ):
     for source in ctx.sources.values():
         validators = await client.list_validators(source._must_id())
 
         for v in validators:
+            if v.resource_namespace != namespace:
+                continue
+
             name = v.resource_name
 
             cls = None
             for c in VALIDATOR_CLASSES:
                 if v.typename__ == c.__name__:
                     cls = c
                     break
```

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/_util.py` & `validio_sdk-0.6.0/validio_sdk/resource/_util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/channels.py` & `validio_sdk-0.6.0/validio_sdk/resource/channels.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/credentials.py` & `validio_sdk-0.6.0/validio_sdk/resource/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/destinations.py` & `validio_sdk-0.6.0/validio_sdk/resource/destinations.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,14 +156,21 @@
 
         self.database = database
         self.db_schema = db_schema
         self.table = table
         self.role = role
         self.warehouse = warehouse
 
+    def __getattr__(self, name):
+        """Getter for field aliases."""
+        # schema is called db_schema
+        if name == "schema":
+            return self.db_schema
+        raise AttributeError
+
     def _mutable_fields(self) -> set[str]:
         return {
             *super()._immutable_fields(),
             *{
                 "database",
                 "db_schema",
                 "table",
```

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/filters.py` & `validio_sdk-0.6.0/validio_sdk/resource/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 class StringFilter(Filter):
     """A String filter configuration.
 
     https://docs.validio.io/docs/filters#string
     """
 
     field: Union[str, "FieldSelector"]
-    value: str
+    value: str | None
     operator: StringFilterOperator
 
     def __post_init__(self):
         """Post init for filter."""
         self.field = self._maybe_set_field_selector("field", self.field)
         if not isinstance(self.operator, StringFilterOperator):
             self.operator = StringFilterOperator(self.operator)
```

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/notification_rules.py` & `validio_sdk-0.6.0/validio_sdk/resource/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/segmentations.py` & `validio_sdk-0.6.0/validio_sdk/resource/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/sources.py` & `validio_sdk-0.6.0/validio_sdk/resource/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from typing import TYPE_CHECKING, Any, Optional, Union, cast
 
 from camel_converter import to_snake
 
 # We need validio_sdk in scope due to eval.
 # ruff: noqa: F401
 import validio_sdk
-from validio_sdk.graphql_client import (
-    CsvParserInput,
-)
+from validio_sdk.graphql_client import CsvParserInput
 from validio_sdk.resource._diffable import Diffable
 from validio_sdk.resource._resource import Resource
 from validio_sdk.resource._serde import (
     CONFIG_FIELD_NAME,
     NODE_TYPE_FIELD_NAME,
     _api_create_input_params,
     _api_update_input_params,
@@ -402,14 +400,16 @@
         }
 
     def _api_infer_schema_input(self) -> dict[str, object] | None:
         return {
             "database": self.database,
             "db_schema": self.db_schema,
             "table": self.table,
+            "role": self.role,
+            "warehouse": self.warehouse,
         }
 
 
 class PostgresLikeSource(Source):
     """A Postgres compatible source configuration."""
 
     def __init__(
@@ -720,25 +720,23 @@
             if csv is None
             else CsvParserConfig._from_any(csv)
         )
 
     def _immutable_fields(self) -> set[str]:
         return {
             *super()._immutable_fields(),
-            *{
-                "bucket",
-                "file_pattern",
-            },
+            *{"bucket"},
         }
 
     def _mutable_fields(self) -> set[str]:
         return {
             *super()._mutable_fields(),
             *{
                 "schedule",
+                "file_pattern",
             },
         }
 
     def _nested_objects(self) -> dict[str, Diffable | None]:
         return {
             "csv": self.csv,
         }
```

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/tests/test__diff.py` & `validio_sdk-0.6.0/validio_sdk/resource/tests/test__diff.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/tests/test__field_selector.py` & `validio_sdk-0.6.0/validio_sdk/resource/tests/test__field_selector.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/tests/test__resource.py` & `validio_sdk-0.6.0/validio_sdk/resource/tests/test__resource.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/thresholds.py` & `validio_sdk-0.6.0/validio_sdk/resource/thresholds.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/validators.py` & `validio_sdk-0.6.0/validio_sdk/resource/validators.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/resource/windows.py` & `validio_sdk-0.6.0/validio_sdk/resource/windows.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/scalars.py` & `validio_sdk-0.6.0/validio_sdk/scalars.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/util.py` & `validio_sdk-0.6.0/validio_sdk/util.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/validio_sdk/validio_client.py` & `validio_sdk-0.6.0/validio_sdk/validio_client.py`

 * *Files identical despite different names*

### Comparing `validio_sdk-0.5.1/PKG-INFO` & `validio_sdk-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-sdk
-Version: 0.5.1
+Version: 0.6.0
 Summary: SDK to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

