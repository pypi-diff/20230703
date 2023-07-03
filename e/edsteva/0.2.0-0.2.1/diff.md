# Comparing `tmp/edsteva-0.2.0.tar.gz` & `tmp/edsteva-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsteva-0.2.0.tar", max compression
+gzip compressed data, was "edsteva-0.2.1.tar", max compression
```

## Comparing `edsteva-0.2.0.tar` & `edsteva-0.2.1.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     1485 2023-06-30 07:53:41.112356 edsteva-0.2.0/LICENSE
--rw-r--r--   0        0        0     2822 2023-06-30 07:53:41.112356 edsteva-0.2.0/README.md
--rw-r--r--   0        0        0     3063 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/__init__.py
--rw-r--r--   0        0        0      138 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/__init__.py
--rw-r--r--   0        0        0     2351 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/files.py
--rw-r--r--   0        0        0    11759 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/hive.py
--rw-r--r--   0        0        0     6209 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/i2b2_mapping.py
--rw-r--r--   0        0        0     2957 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/postgres.py
--rw-r--r--   0        0        0    11528 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/settings.py
--rw-r--r--   0        0        0       37 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/__init__.py
--rw-r--r--   0        0        0     3766 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/biology.py
--rw-r--r--   0        0        0     1053 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/care_site.py
--rw-r--r--   0        0        0     3994 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/note.py
--rw-r--r--   0        0        0    26222 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/synthetic.py
--rw-r--r--   0        0        0     2814 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/utils.py
--rw-r--r--   0        0        0     3557 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/visit.py
--rw-r--r--   0        0        0      395 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/__init__.py
--rw-r--r--   0        0        0     2169 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/error.py
--rw-r--r--   0        0        0     2558 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/error_after_t0.py
--rw-r--r--   0        0        0     2718 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/error_between_t0_t1.py
--rw-r--r--   0        0        0       42 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/__init__.py
--rw-r--r--   0        0        0    10953 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/base.py
--rw-r--r--   0        0        0       83 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/__init__.py
--rw-r--r--   0        0        0      239 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/algos/__init__.py
--rw-r--r--   0        0        0     3325 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     5621 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/rectangle_function.py
--rw-r--r--   0        0        0     1450 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/__init__.py
--rw-r--r--   0        0        0     5197 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/defaults.py
--rw-r--r--   0        0        0     1271 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
--rw-r--r--   0        0        0     1110 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
--rw-r--r--   0        0        0      336 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
--rw-r--r--   0        0        0      207 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/probe_plot.py
--rw-r--r--   0        0        0       68 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/__init__.py
--rw-r--r--   0        0        0      336 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/algos/__init__.py
--rw-r--r--   0        0        0     2666 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     2528 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/algos/quantile.py
--rw-r--r--   0        0        0     5292 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/step_function.py
--rw-r--r--   0        0        0     1395 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/__init__.py
--rw-r--r--   0        0        0     4315 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/defaults.py
--rw-r--r--   0        0        0     1024 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      863 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
--rw-r--r--   0        0        0      336 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/probe_dashboard.py
--rw-r--r--   0        0        0      207 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/probe_plot.py
--rw-r--r--   0        0        0      257 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/__init__.py
--rw-r--r--   0        0        0    14033 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/base.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/__init__.py
--rw-r--r--   0        0        0     9091 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/biology.py
--rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     5688 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/per_measurement.py
--rw-r--r--   0        0        0     6468 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     2595 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
--rw-r--r--   0        0        0     5642 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
--rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
--rw-r--r--   0        0        0      693 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
--rw-r--r--   0        0        0      568 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
--rw-r--r--   0        0        0     5941 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
--rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
--rw-r--r--   0        0        0      693 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
--rw-r--r--   0        0        0      568 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     5963 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      693 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      568 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/__init__.py
--rw-r--r--   0        0        0      483 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     7947 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_condition.py
--rw-r--r--   0        0        0     8932 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     6392 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/condition.py
--rw-r--r--   0        0        0     2437 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/__init__.py
--rw-r--r--   0        0        0     5701 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/__init__.py
--rw-r--r--   0        0        0     5933 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     6549 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/note/__init__.py
--rw-r--r--   0        0        0      457 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/note/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     7259 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_note.py
--rw-r--r--   0        0        0     8556 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     6418 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/note.py
--rw-r--r--   0        0        0     2278 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/__init__.py
--rw-r--r--   0        0        0     5218 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/__init__.py
--rw-r--r--   0        0        0     5475 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     6185 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/__init__.py
--rw-r--r--   0        0        0    10772 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/filter_df.py
--rw-r--r--   0        0        0    22364 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/prepare_df.py
--rw-r--r--   0        0        0     6796 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/__init__.py
--rw-r--r--   0        0        0      291 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     8269 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     5326 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/visit.py
--rw-r--r--   0        0        0     1795 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/__init__.py
--rw-r--r--   0        0        0     4982 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
--rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     5237 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/__init__.py
--rw-r--r--   0        0        0     2498 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/checks.py
--rw-r--r--   0        0        0     1108 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/file_management.py
--rw-r--r--   0        0        0     2050 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/framework.py
--rw-r--r--   0        0        0      176 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/loss_functions.py
--rw-r--r--   0        0        0      344 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/typing.py
--rw-r--r--   0        0        0       52 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/__init__.py
--rw-r--r--   0        0        0      242 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/normalized_probe/__init__.py
--rw-r--r--   0        0        0    11510 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/__init__.py
--rw-r--r--   0        0        0     4251 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/fitted_probe.py
--rw-r--r--   0        0        0     3496 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/probe.py
--rw-r--r--   0        0        0     7720 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/wrapper.py
--rw-r--r--   0        0        0      339 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/estimates_densities/__init__.py
--rw-r--r--   0        0        0     8510 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/estimates_densities/estimates_densities.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/normalized_probe/__init__.py
--rw-r--r--   0        0        0     7491 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/normalized_probe/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/__init__.py
--rw-r--r--   0        0        0     2334 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/fitted_probe.py
--rw-r--r--   0        0        0     1483 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/probe.py
--rw-r--r--   0        0        0     5473 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/wrapper.py
--rw-r--r--   0        0        0    16085 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/utils.py
--rw-r--r--   0        0        0     3307 2023-06-30 07:53:41.132357 edsteva-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 edsteva-0.2.0/setup.py
--rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 edsteva-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-07-03 12:48:49.034275 edsteva-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2822 2023-07-03 12:48:49.034275 edsteva-0.2.1/README.md
+-rw-r--r--   0        0        0     3083 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/__init__.py
+-rw-r--r--   0        0        0     2345 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/files.py
+-rw-r--r--   0        0        0    11701 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/hive.py
+-rw-r--r--   0        0        0     6221 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/i2b2_mapping.py
+-rw-r--r--   0        0        0     2957 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/postgres.py
+-rw-r--r--   0        0        0     9050 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/settings.py
+-rw-r--r--   0        0        0       37 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/__init__.py
+-rw-r--r--   0        0        0     4044 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/biology.py
+-rw-r--r--   0        0        0     1053 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/care_site.py
+-rw-r--r--   0        0        0     4169 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/note.py
+-rw-r--r--   0        0        0    27017 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/synthetic.py
+-rw-r--r--   0        0        0     2997 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/utils.py
+-rw-r--r--   0        0        0     3835 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/io/synthetic/visit.py
+-rw-r--r--   0        0        0      395 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/metrics/__init__.py
+-rw-r--r--   0        0        0     2169 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/metrics/error.py
+-rw-r--r--   0        0        0     2558 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/metrics/error_after_t0.py
+-rw-r--r--   0        0        0     2718 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/metrics/error_between_t0_t1.py
+-rw-r--r--   0        0        0       42 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/__init__.py
+-rw-r--r--   0        0        0    10800 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/base.py
+-rw-r--r--   0        0        0       83 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/__init__.py
+-rw-r--r--   0        0        0      239 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/algos/__init__.py
+-rw-r--r--   0        0        0     3329 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     5590 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/rectangle_function.py
+-rw-r--r--   0        0        0     1450 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     5197 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0     1207 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0     1036 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      284 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      165 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0       68 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/algos/__init__.py
+-rw-r--r--   0        0        0     2670 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     2488 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/algos/quantile.py
+-rw-r--r--   0        0        0     5292 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/step_function.py
+-rw-r--r--   0        0        0     1395 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     4315 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0      960 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      789 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      284 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      165 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/models/step_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0      257 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/__init__.py
+-rw-r--r--   0        0        0    14067 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/base.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/__init__.py
+-rw-r--r--   0        0        0     9091 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/biology.py
+-rw-r--r--   0        0        0      488 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     5645 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/completeness_predictors/per_measurement.py
+-rw-r--r--   0        0        0     6468 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     2595 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
+-rw-r--r--   0        0        0     5642 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      618 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
+-rw-r--r--   0        0        0     5941 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      618 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5963 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      618 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/__init__.py
+-rw-r--r--   0        0        0      483 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7900 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/completeness_predictors/per_condition.py
+-rw-r--r--   0        0        0     8932 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6392 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/condition.py
+-rw-r--r--   0        0        0     2437 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.046276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/__init__.py
+-rw-r--r--   0        0        0     5701 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/__init__.py
+-rw-r--r--   0        0        0     5933 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     6549 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7222 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/completeness_predictors/per_note.py
+-rw-r--r--   0        0        0     8556 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6418 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/note.py
+-rw-r--r--   0        0        0     2278 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/__init__.py
+-rw-r--r--   0        0        0     5218 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/__init__.py
+-rw-r--r--   0        0        0     5475 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     6185 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/utils/__init__.py
+-rw-r--r--   0        0        0    10772 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/utils/filter_df.py
+-rw-r--r--   0        0        0    22314 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/utils/prepare_df.py
+-rw-r--r--   0        0        0     6672 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     8230 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     5326 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/visit.py
+-rw-r--r--   0        0        0     1795 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/__init__.py
+-rw-r--r--   0        0        0     4982 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5237 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      486 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      244 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/utils/__init__.py
+-rw-r--r--   0        0        0     2498 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/utils/checks.py
+-rw-r--r--   0        0        0     1155 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/utils/file_management.py
+-rw-r--r--   0        0        0     1970 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/utils/framework.py
+-rw-r--r--   0        0        0      176 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/utils/loss_functions.py
+-rw-r--r--   0        0        0      344 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/utils/typing.py
+-rw-r--r--   0        0        0       52 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/normalized_probe/__init__.py
+-rw-r--r--   0        0        0    11510 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/probe/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/probe/fitted_probe.py
+-rw-r--r--   0        0        0     3477 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/probe/probe.py
+-rw-r--r--   0        0        0     7686 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/dashboards/probe/wrapper.py
+-rw-r--r--   0        0        0      339 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/estimates_densities/__init__.py
+-rw-r--r--   0        0        0     8510 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/estimates_densities/estimates_densities.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/normalized_probe/__init__.py
+-rw-r--r--   0        0        0     7491 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/probe/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/probe/fitted_probe.py
+-rw-r--r--   0        0        0     1483 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/probe/probe.py
+-rw-r--r--   0        0        0     5473 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/plots/probe/wrapper.py
+-rw-r--r--   0        0        0    15945 2023-07-03 12:48:49.050276 edsteva-0.2.1/edsteva/viz/utils.py
+-rw-r--r--   0        0        0     3492 2023-07-03 12:48:49.054276 edsteva-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 edsteva-0.2.1/setup.py
+-rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 edsteva-0.2.1/PKG-INFO
```

### Comparing `edsteva-0.2.0/LICENSE` & `edsteva-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/README.md` & `edsteva-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.2.0
+pip install edsteva==0.2.1
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.2.0 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.1 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

### Comparing `edsteva-0.2.0/edsteva/__init__.py` & `edsteva-0.2.1/edsteva/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 import importlib
 import os
 import sys
 import time
 from distutils.version import LooseVersion
@@ -26,15 +26,15 @@
 
     # Reloading Koalas to use the new configuration
     ks = sys.modules.get("databricks.koalas", None)
 
     if ks is not None:
         importlib.reload(ks)
 
-    else:
+    else:  # pragma: no cover
         import databricks.koalas as ks
 
     ks.set_option("compute.default_index_type", "distributed")
     ks.set_option("compute.ops_on_diff_frames", True)
 
 
 def set_env_variables() -> None:
```

### Comparing `edsteva-0.2.0/edsteva/io/files.py` & `edsteva-0.2.1/edsteva/io/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 from typing import List, Tuple
 
 import pandas as pd
 
 from . import settings
 
 
@@ -46,31 +47,30 @@
     @staticmethod
     def list_available_tables(folder: str) -> Tuple[List[str], List[str]]:
         available_tables = []
         available_omop_tables = []
         tables_paths = {}
         known_omop_tables = settings.tables_to_load.keys()
         for filename in os.listdir(folder):
-            table_name, extension = os.path.splitext(filename)
+            file = Path(folder) / filename
+            table_name = file.stem
+            extension = file.suffix
             if extension == ".parquet":
-                abspath = os.path.abspath(os.path.join(folder, filename))
+                abspath = Path.resolve(file)
                 tables_paths[table_name] = abspath
                 available_tables.append(table_name)
                 if table_name in known_omop_tables:
                     available_omop_tables.append(table_name)
 
         return available_tables, tables_paths, available_omop_tables
 
     def _read_table(self, table_name: str) -> pd.DataFrame:
         path = self.tables_paths[table_name]
         return pd.read_parquet(path)
 
     def __getattr__(self, table_name: str) -> pd.DataFrame:
         if table_name in self.available_tables:
             return self._read_table(table_name)
-        else:
-            raise AttributeError(
-                f"Table '{table_name}' does is not available in chosen folder."
-            )
+        raise AttributeError(f"Table '{table_name}' is not available in chosen folder.")
 
     def __dir__(self) -> List[str]:
         return list(super().__dir__()) + list(self.available_tables)
```

### Comparing `edsteva-0.2.0/edsteva/io/hive.py` & `edsteva-0.2.1/edsteva/io/hive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 from typing import Dict, Iterable, List, Optional, Union
 
 import pandas
 from databricks import koalas
 from loguru import logger
 from pyspark.sql import DataFrame as SparkDataFrame
 from pyspark.sql import SparkSession
@@ -195,27 +195,26 @@
         self.tables_to_load.pop(table_name, None)
         self.available_tables = self.list_available_tables()
         logger.info("Table {} has been deleted", table_name)
 
     def _prepare_person_ids(self, list_of_person_ids) -> Optional[SparkDataFrame]:
         if list_of_person_ids is None:
             return None
-        elif hasattr(list_of_person_ids, "to_list"):
+        if hasattr(list_of_person_ids, "to_list"):
             # Useful when list_of_person_ids are Koalas (or Pandas) Series
             unique_ids = set(list_of_person_ids.to_list())
         else:
             unique_ids = set(list_of_person_ids)
 
         logger.info("Number of unique patients: {}", len(unique_ids))
         schema = StructType([StructField("person_id", LongType(), True)])
 
-        filtering_df = self.spark_session.createDataFrame(
+        return self.spark_session.createDataFrame(
             [(int(p),) for p in unique_ids], schema=schema
         )
-        return filtering_df
 
     def _read_table(self, table_name, person_ids=None) -> DataFrame:
         assert table_name in self.available_tables
         if person_ids is None and self.person_ids is not None:
             person_ids = self.person_ids
 
         if self.database_type == "OMOP":
@@ -267,44 +266,43 @@
             tables = settings.default_tables_to_save
 
         unknown_tables = [
             table for table in tables if table not in self.available_tables
         ]
         if unknown_tables:
             raise ValueError(
-                f"The following tables are not available : {str(unknown_tables)}"
+                f"The following tables are not available : {unknown_tables}"
             )
 
-        folder = os.path.abspath(folder)
-        assert os.path.exists(folder) and os.path.isdir(
+        folder = Path.resolve(folder)
+        assert Path.exists(folder) and Path.is_dir(
             folder
         ), f"Folder {folder} not found."
 
         if person_ids is not None:
             person_ids = self._prepare_person_ids(person_ids)
 
         for table in tables:
-            filepath = os.path.join(folder, f"{table}.parquet")
+            filepath = folder / f"{table}.parquet"
             df = self._read_table(table, person_ids=person_ids)
             self._write_df_to_parquet(df, filepath)
 
     def _write_df_to_parquet(
         self,
         df: DataFrame,
         filepath: str,
     ) -> None:
-        assert os.path.isabs(filepath)
-        print(f"writing {filepath}")
+        assert Path.is_absolute(filepath)
+        logger.info(f"writing {filepath}")
         spark_filepath = "file://" + filepath
         df.to_parquet(spark_filepath, mode="overwrite")
 
     def __getattr__(self, table_name: str) -> DataFrame:
         if table_name in self.available_tables:
             # the first time it is called, we actually set the attribute
             table = self._read_table(table_name)
             setattr(self, table_name, table)
             return getattr(self, table_name)
-        else:
-            raise AttributeError(f"Table '{table_name}' unknown")
+        raise AttributeError(f"Table '{table_name}' unknown")
 
     def __dir__(self) -> List[str]:
         return list(set(list(super().__dir__()) + self.available_tables))
```

### Comparing `edsteva-0.2.0/edsteva/io/i2b2_mapping.py` & `edsteva-0.2.1/edsteva/io/i2b2_mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -164,31 +164,31 @@
         # Only UF-Hospital relationships in i2b2
         df = df.withColumn("relationship_concept_id", F.lit(46233688))  # Included in
 
     return df
 
 
 def mapping_dict(
-    mapping: Dict[str, str], Non_renseigne: str
+    mapping: Dict[str, str], not_specified_val: str
 ) -> FunctionUDF:  # pragma: no cover
     """
     Returns a function that maps data according to a mapping dictionnary in a Spark DataFrame.
 
     Parameters
     ----------
     mapping: Dict
         Mapping dictionnary
-    Non_renseigne: str
+    not_specified_val: str
         Value to return if the function input is not find in the mapping dictionnary.
 
     Returns
     -------
     Callable
         Function that maps the values of Spark DataFrame column.
     """
 
     def f(x):
         if x in mapping:
             return mapping.get(x)
-        return Non_renseigne
+        return not_specified_val
 
     return F.udf(f)
```

### Comparing `edsteva-0.2.0/edsteva/io/postgres.py` & `edsteva-0.2.1/edsteva/io/postgres.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/io/settings.py` & `edsteva-0.2.1/edsteva/io/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,205 +1,126 @@
+"""
+The default tables loaded when instanciating a [``HiveData``][edsteva.io.hive.HiveData]
+or a [``PostgresData``][edsteva.io.postgres.PostgresData]
+"""
 default_tables_to_save = [
     "person",
     "visit_occurrence",
     "visit_detail",
     "condition_occurrence",
     "procedure_occurrence",
     "care_site",
     "concept",
 ]
+
 """
-The default tables loaded when instanciating a [``HiveData``][edsteva.io.hive.HiveData]
+The default columns loaded when instanciating a [``HiveData``][edsteva.io.hive.HiveData]
 or a [``PostgresData``][edsteva.io.postgres.PostgresData]
 """
-
 tables_to_load = {
     "person": [
-        # "key",
         "person_id",
-        # "person_source_value",
         "location_id",
-        # "provider_id",
-        # "care_site_id",
         "year_of_birth",
         "month_of_birth",
         "day_of_birth",
         "birth_datetime",
         "death_datetime",
-        # "race_concept_id",
-        # "race_source_value",
-        # "race_source_concept_id",
-        # "ethnicity_concept_id",
-        # "ethnicity_source_value",
-        # "ethnicity_source_concept_id",
-        # "gender_concept_id",
         "gender_source_value",
         "gender_source_concept_id",
-        # "row_status_concept_id",
-        # "row_status_source_value",
-        # "row_status_source_concept_id",
+        "status_source_value",
         "cdm_source",
     ],
     "visit_occurrence": [
-        # "key",
         "visit_occurrence_id",
         "person_id",
         "visit_occurrence_source_value",
         "preceding_visit_occurrence_id",
-        # "provider_id",
         "care_site_id",
-        # "visit_start_date",
         "visit_start_datetime",
-        # "visit_end_date",
         "visit_end_datetime",
-        # "visit_concept_id",
         "visit_source_value",
         "visit_source_concept_id",
-        # "visit_type_concept_id",
         "visit_type_source_value",
         "visit_type_source_concept_id",
-        # "admitted_from_concept_id",
         "admitted_from_source_value",
         "admitted_from_source_concept_id",
-        # "discharge_to_concept_id",
         "discharge_to_source_value",
         "discharge_to_source_concept_id",
-        # "row_status_concept_id",
         "row_status_source_value",
-        # "row_status_source_concept_id",
-        # "stay_concept_id",
         "stay_source_value",
         "stay_source_concept_id",
         "cdm_source",
     ],
     "care_site": [
-        # "key",
         "care_site_id",
         "care_site_source_value",
-        # "location_id",
         "care_site_name",
         "care_site_short_name",
-        # "place_of_service_concept_id",
         "place_of_service_source_value",
-        # "place_of_service_source_concept_id",
-        # "care_site_type_concept_id",
         "care_site_type_source_value",
-        # "care_site_type_source_concept_id",
         "valid_start_date",
         "valid_end_date",
-        # "cdm_source",
     ],
     "visit_detail": [
-        # "key",
         "visit_detail_id",
         "visit_occurrence_id",
         "person_id",
         "preceding_visit_detail_id",
         "visit_detail_parent_id",
-        # "provider_id",
         "care_site_id",
         "visit_detail_start_date",
         "visit_detail_start_datetime",
         "visit_detail_end_date",
         "visit_detail_end_datetime",
-        # "visit_detail_concept_id",
         "visit_detail_source_value",
         "visit_detail_source_concept_id",
-        # "visit_detail_type_concept_id",
         "visit_detail_type_source_value",
         "visit_detail_type_source_concept_id",
-        # "admitted_from_concept_id",
         "admitted_from_source_value",
         "admitted_from_source_concept_id",
-        # "discharge_to_concept_id",
         "discharge_to_source_value",
         "discharge_to_source_concept_id",
-        # "row_status_concept_id",
-        # "row_status_source_value",
-        # "row_status_source_concept_id",
         "cdm_source",
     ],
     "condition_occurrence": [
-        # "key",
         "condition_occurrence_id",
         "person_id",
         "visit_occurrence_id",
         "visit_detail_id",
-        # "provider_id",
-        # "condition_start_date",
         "condition_start_datetime",
-        # "condition_end_date",
-        # "condition_end_datetime",
-        # "condition_concept_id",
         "condition_source_value",
         "condition_source_concept_id",
-        # "condition_type_concept_id",
-        # "condition_type_source_value",
-        # "condition_type_source_concept_id",
-        # "condition_status_concept_id",
         "condition_status_source_value",
         "condition_status_source_concept_id",
-        # "stop_reason",
-        # "row_status_concept_id",
-        # "row_status_source_value",
-        # "row_status_source_concept_id",
         "cdm_source",
     ],
     "procedure_occurrence": [
-        # "key",
         "procedure_occurrence_id",
         "person_id",
         "visit_occurrence_id",
         "visit_detail_id",
-        # "provider_id",
-        # "procedure_date",
         "procedure_datetime",
-        # "procedure_concept_id",
         "procedure_source_value",
         "procedure_source_concept_id",
-        # "procedure_type_concept_id",
-        # "procedure_type_source_value",
-        # "procedure_type_source_concept_id",
-        # "modifier_concept_id",
-        # "modifier_source_value",
-        # "quantity",
-        # "row_status_concept_id",
-        # "row_status_source_value",
-        # "row_status_source_concept_id",
         "cdm_source",
     ],
-    # "note": [],
-    # "location": [],
-    # location_history
-    # measurement
-    # drug_exposure
-    # note_nlp
-    # observation
     "concept": [
         "concept_id",
         "concept_name",
         "domain_id",
         "vocabulary_id",
         "concept_class_id",
         "standard_concept",
         "concept_code",
         "valid_start_date",
         "valid_end_date",
         "invalid_reason",
-        # "hash",
     ],
-    # concept_relationship
-    # concept_synonym
-    # fact_relationship
-    # vocabulary
 }
-"""
-The default columns loaded when instanciating a [``HiveData``][edsteva.io.hive.HiveData]
-or a [``PostgresData``][edsteva.io.postgres.PostgresData]
-"""
 
 
 # make sure we know how to load the tables we want to save
 assert all(table in tables_to_load.keys() for table in default_tables_to_save)
 
 """
 The available tables from i2b2 and their mapping to OMOP standard.
```

### Comparing `edsteva-0.2.0/edsteva/io/synthetic/biology.py` & `edsteva-0.2.1/edsteva/io/synthetic/biology.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,60 +8,65 @@
     generate_events_around_t0,
     generate_events_around_t1,
     generate_events_before_t0,
 )
 
 
 def generate_bio(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     increase_time: int,
     increase_ratio: float,
     bio_date_col: str,
     unit: str,
     concept_code: str,
     mode: str,
 ):
     if mode == "step":
         return _generate_bio_step(
+            generator=generator,
             t_start=t_start,
             t_end=t_end,
             n_events=n_events,
             increase_time=increase_time,
             increase_ratio=increase_ratio,
             bio_date_col=bio_date_col,
             unit=unit,
             concept_code=concept_code,
         )
     if mode == "rect":
         return _generate_bio_rect(
+            generator=generator,
             t_start=t_start,
             t_end=t_end,
             n_events=n_events,
             increase_time=increase_time,
             increase_ratio=increase_ratio,
             bio_date_col=bio_date_col,
             unit=unit,
             concept_code=concept_code,
         )
 
 
 def _generate_bio_step(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     increase_time: int,
     increase_ratio: float,
     bio_date_col: str,
     unit: str,
     concept_code: str,
 ):
-    t0 = np.random.randint(t_start + increase_time, t_end - increase_time)
+    t0 = generator.integers(t_start + increase_time, t_end - increase_time)
     params = dict(
+        generator=generator,
         t_start=t_start,
         t_end=t_end,
         n_events=n_events,
         t0=t0,
         increase_ratio=increase_ratio,
         increase_time=increase_time,
     )
@@ -79,40 +84,45 @@
     df["t_0_max"] = t0 + increase_time / 2
     logger.debug("Generate measurement deploying as step function")
 
     return df
 
 
 def _generate_bio_rect(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     increase_time: int,
     increase_ratio: float,
     bio_date_col: str,
     unit: str,
     concept_code: str,
 ):
-    t0 = np.random.randint(
+    t0 = generator.integers(
         t_start + increase_time, (t_end + t_start) / 2 - increase_time
     )
-    t1 = np.random.randint((t_end + t_start) / 2 + increase_time, t_end - increase_time)
+    t1 = generator.integers(
+        (t_end + t_start) / 2 + increase_time, t_end - increase_time
+    )
     t0_params = dict(
+        generator=generator,
         t_start=t_start,
         t_end=t1 - increase_time / 2,
         n_events=n_events,
         t0=t0,
         increase_ratio=increase_ratio,
         increase_time=increase_time,
     )
     before_t0 = generate_events_before_t0(**t0_params)
     around_t0 = generate_events_around_t0(**t0_params)
     # Raise n_visit to enforce a rectangle shape
     between_t0_t1 = generate_events_after_t0(**t0_params)
     t1_params = dict(
+        generator=generator,
         t_start=t_start,
         t_end=t_end,
         n_events=n_events,
         t1=t1,
         increase_time=increase_time,
         increase_ratio=increase_ratio,
     )
```

### Comparing `edsteva-0.2.0/edsteva/io/synthetic/care_site.py` & `edsteva-0.2.1/edsteva/io/synthetic/care_site.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/io/synthetic/note.py` & `edsteva-0.2.1/edsteva/io/synthetic/note.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 import numpy as np
 import pandas as pd
 from loguru import logger
 
 
 def generate_note(
+    generator: np.random.Generator,
     visit_care_site: pd.DataFrame,
     note_type: str,
     note_date_col: str,
     id_visit_col: str,
     note_type_col: str,
     t0_visit: int,
     care_site_id: int,
     date_col: str,
     mode: str,
 ):
     if mode == "step":
         return _generate_note_step(
+            generator=generator,
             visit_care_site=visit_care_site,
             note_type=note_type,
             note_date_col=note_date_col,
             id_visit_col=id_visit_col,
             note_type_col=note_type_col,
             t0_visit=t0_visit,
             care_site_id=care_site_id,
             date_col=date_col,
         )
 
-    elif mode == "rect":
+    if mode == "rect":
         return _generate_note_rect(
+            generator=generator,
             visit_care_site=visit_care_site,
             note_type=note_type,
             note_date_col=note_date_col,
             id_visit_col=id_visit_col,
             note_type_col=note_type_col,
             t0_visit=t0_visit,
             care_site_id=care_site_id,
             date_col=date_col,
         )
 
 
 def _generate_note_step(
+    generator: np.random.Generator,
     visit_care_site,
     note_type,
     care_site_id,
     date_col,
     note_date_col,
     id_visit_col,
     note_type_col,
     t0_visit,
 ):
     t_end = visit_care_site[date_col].max()
-    t0 = np.random.randint(t0_visit, t_end)
-    c_before = np.random.uniform(0, 0.2)
-    c_after = np.random.uniform(0.8, 1)
+    t0 = generator.integers(t0_visit, t_end)
+    c_before = generator.uniform(0, 0.2)
+    c_after = generator.uniform(0.8, 1)
     note_before_t0_visit = (
         visit_care_site[visit_care_site[date_col] <= t0_visit][[id_visit_col, date_col]]
         .sample(frac=c_before)
         .rename(columns={date_col: note_date_col})
     )
     # Stratify visit between t0_visit and t0 to
     # ensure that these elements are represented
@@ -83,28 +87,29 @@
     note["t_0"] = t0
     logger.debug("Generate synthetic note deploying as step function")
 
     return note
 
 
 def _generate_note_rect(
+    generator: np.random.Generator,
     visit_care_site,
     note_type,
     care_site_id,
     date_col,
     note_date_col,
     id_visit_col,
     note_type_col,
     t0_visit,
 ):
     t1_visit = visit_care_site["t_1_min"].max()
-    t0 = np.random.randint(t0_visit, t0_visit + (t1_visit - t0_visit) / 3)
-    t1 = np.random.randint(t0_visit + 2 * (t1_visit - t0_visit) / 3, t1_visit)
-    c_out = np.random.uniform(0, 0.1)
-    c_in = np.random.uniform(0.8, 1)
+    t0 = generator.integers(t0_visit, t0_visit + (t1_visit - t0_visit) / 3)
+    t1 = generator.integers(t0_visit + 2 * (t1_visit - t0_visit) / 3, t1_visit)
+    c_out = generator.uniform(0, 0.1)
+    c_in = generator.uniform(0.8, 1)
 
     note_before_t0 = (
         visit_care_site[visit_care_site[date_col] <= t0][[id_visit_col, date_col]]
         .sample(frac=c_out)
         .rename(columns={date_col: note_date_col})
     )
     note_between_t0_t1 = (
```

### Comparing `edsteva-0.2.0/edsteva/io/synthetic/synthetic.py` & `edsteva-0.2.1/edsteva/io/synthetic/synthetic.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,18 +116,22 @@
         ("Attendu", 0.02),
         ("Confirmé", 0.02),
         ("Initial", 0.02),
     ],
 )
 
 
-def add_other_columns(table: pd.DataFrame, other_columns: Dict):
+def add_other_columns(
+    generator: np.random.Generator,
+    table: pd.DataFrame,
+    other_columns: Dict,
+):
     for name, params in other_columns.items():
         options, prob = list(zip(*params))
-        table[name] = pd.Series(np.random.choice(options, size=len(table), p=prob))
+        table[name] = pd.Series(generator.choice(options, size=len(table), p=prob))
     return table
 
 
 @dataclass
 class SyntheticData:
     module: str = "pandas"
     mean_visit: int = 1000
@@ -156,23 +160,27 @@
         default_factory=lambda: OTHER_MEASUREMENT_COLUMNS
     )
     seed: int = None
     mode: str = "step"
 
     def __post_init__(self):
         if self.module not in ["pandas", "koalas"]:
-            raise ValueError(
+            raise AttributeError(
                 f"Unknown module {self.mode}, options are ('pandas', 'koalas')"
             )
         if self.mode not in ["step", "rect"]:
-            raise ValueError(f"Unknown mode {self.mode}, options are ('step', 'rect')")
+            raise AttributeError(
+                f"Unknown mode {self.mode}, options are ('step', 'rect')"
+            )
 
     def generate(self):
         if self.seed:
-            np.random.seed(seed=self.seed)
+            self.generator = np.random.default_rng(self.seed)
+        else:
+            self.generator = np.random.default_rng()
 
         care_site, fact_relationship, hospital_ids = self._generate_care_site_tables()
         visit_occurrence = self._generate_visit_occurrence(hospital_ids)
         visit_detail = self._generate_visit_detail(visit_occurrence, care_site)
         condition_occurrence = self._generate_condition_occurrence(
             visit_detail,
         )
@@ -202,57 +210,60 @@
 
     def _generate_care_site_tables(self):
         care_site, fact_relationship = generate_care_site_tables(CARE_SITE_STRUCTURE)
         uc_care_site = care_site[
             care_site.care_site_type_source_value == "Unité de consultation (UC)"
         ][["care_site_id"]].reset_index(drop=True)
         uc_care_site = add_other_columns(
-            uc_care_site,
+            generator=self.generator,
+            table=uc_care_site,
             other_columns=dict(
                 place_of_service_source_value=[
                     ("CARDIO", 0.2),
                     ("PEDIATRIE", 0.4),
                     ("PSYCHIATRIE", 0.4),
                 ]
             ),
         )
         uh_care_site = care_site[
             care_site.care_site_type_source_value == "Unité d’hébergement (UH)"
         ][["care_site_id"]].reset_index(drop=True)
         uh_care_site = add_other_columns(
-            uh_care_site,
+            generator=self.generator,
+            table=uh_care_site,
             other_columns=dict(
                 place_of_service_source_value=[
                     ("REA ADULTE", 0.5),
                     ("USI ADULTE", 0.5),
                 ]
             ),
         )
         care_site = care_site.merge(
             pd.concat([uc_care_site, uh_care_site]), on="care_site_id", how="left"
         )
-        care_site.fillna("Non Renseigné", inplace=True)
+        care_site = care_site.fillna("Non Renseigné")
         hospital_ids = list(
             care_site[care_site.care_site_type_source_value == "Hôpital"].care_site_id
         )
         return care_site, fact_relationship, hospital_ids
 
     def _generate_visit_occurrence(self, hospital_ids):
         visit_occurrence = []
         t_min = self.t_min.timestamp()
         t_max = self.t_max.timestamp()
         for care_site_id in hospital_ids:
-            t_start = t_min + np.random.randint(0, (t_max - t_min) / 20)
-            t_end = t_max - np.random.randint(0, (t_max - t_min) / 20)
-            n_visits = np.random.normal(self.mean_visit, self.mean_visit / 5)
-            increase_time = np.random.randint(
+            t_start = t_min + self.generator.integers(0, (t_max - t_min) / 20)
+            t_end = t_max - self.generator.integers(0, (t_max - t_min) / 20)
+            n_visits = self.generator.normal(self.mean_visit, self.mean_visit / 5)
+            increase_time = self.generator.integers(
                 (t_end - t_start) / 100, (t_end - t_start) / 10
             )
-            increase_ratio = np.random.uniform(150, 200)
+            increase_ratio = self.generator.uniform(150, 200)
             params = dict(
+                generator=self.generator,
                 t_start=t_start,
                 t_end=t_end,
                 n_events=n_visits,
                 increase_ratio=increase_ratio,
                 increase_time=increase_time,
                 care_site_id=care_site_id,
                 date_col=self.date_col,
@@ -262,63 +273,68 @@
             visit_occurrence.append(vo_stays)
 
         visit_occurrence = pd.concat(visit_occurrence).reset_index(drop=True)
         visit_occurrence[self.end_date_col] = visit_occurrence[
             self.date_col
         ] + pd.to_timedelta(
             pd.Series(
-                np.random.choice([None] * 50 + list(range(100)), len(visit_occurrence))
+                self.generator.choice(
+                    [None] * 50 + list(range(100)), len(visit_occurrence)
+                )
             ),
             unit="days",
         )
         visit_occurrence[self.id_visit_col] = range(visit_occurrence.shape[0])
         visit_occurrence[self.id_visit_source_col] = range(visit_occurrence.shape[0])
-        visit_occurrence = add_other_columns(visit_occurrence, self.other_visit_columns)
-
-        return visit_occurrence
+        return add_other_columns(
+            generator=self.generator,
+            table=visit_occurrence,
+            other_columns=self.other_visit_columns,
+        )
 
     def _generate_visit_detail(self, visit_occurrence, care_site):
         t_min = self.t_min.timestamp()
         t_max = self.t_max.timestamp()
         visit_detail = []
         cols = visit_occurrence.columns
         col_to_idx = dict(zip(cols, range(len(cols))))
 
-        for visit in visit_occurrence.values:
-            n_visit_detail = np.random.randint(1, 5)
+        for visit in visit_occurrence.to_numpy():
+            n_visit_detail = self.generator.integers(1, 5)
             visit_date_start = visit[col_to_idx[self.date_col]].timestamp()
             visit_date_end = min(visit_date_start + (t_max - t_min) / 50, t_max)
             visit_id = visit[col_to_idx["visit_occurrence_id"]]
             hospital_id = visit[col_to_idx["care_site_id"]]
             uf_ids = [
                 uf.split("-")[1]
                 for uf in recursive_items(
                     CARE_SITE_STRUCTURE["Hôpital-{}".format(hospital_id)]
                 )
             ]
-            care_site_ids = np.random.choice(uf_ids, n_visit_detail)
+            care_site_ids = self.generator.choice(uf_ids, n_visit_detail)
             detail = pd.DataFrame(
                 {
                     self.id_visit_col: visit_id,
                     self.detail_date_col: pd.to_datetime(
-                        np.random.randint(
+                        self.generator.integers(
                             visit_date_start, visit_date_end, n_visit_detail
                         ),
                         unit="s",
                     ),
                     "care_site_id": care_site_ids,
                 }
             )
             visit_detail.append(detail)
 
         visit_detail = pd.concat(visit_detail).reset_index(drop=True)
         visit_detail[self.id_detail_col] = range(visit_detail.shape[0])
         visit_detail = add_other_columns(
-            visit_detail,
-            self.other_detail_columns,
+            generator=self.generator,
+            table=visit_detail,
+            other_columns=self.other_detail_columns,
         )
         visit_detail = visit_detail.merge(care_site, on="care_site_id")
         uc_detail = (
             visit_detail[
                 visit_detail.care_site_type_source_value == "Unité de consultation (UC)"
             ]
             .copy()
@@ -341,29 +357,28 @@
             .reset_index(drop=True)
         )
         uf_detail["visit_detail_type_source_value"] = "PASS UF"
         rum_detail = uf_detail.copy()
         rum_detail["visit_detail_type_source_value"] = "RUM"
         care_site_col = list(care_site.columns)
         care_site_col.remove("care_site_id")
-        visit_detail = pd.concat([uc_detail, uh_detail, uf_detail, rum_detail]).drop(
+        return pd.concat([uc_detail, uh_detail, uf_detail, rum_detail]).drop(
             columns=care_site_col
         )
-        return visit_detail
 
     def _generate_condition_occurrence(self, visit_detail):
         visit_detail = visit_detail[
             visit_detail.visit_detail_type_source_value == "RUM"
         ]
         condition_occurrence = []
         cols = visit_detail.columns
         col_to_idx = dict(zip(cols, range(len(cols))))
 
-        for visit in visit_detail.values:
-            n_condition = np.random.randint(1, 5)
+        for visit in visit_detail.to_numpy():
+            n_condition = self.generator.integers(1, 5)
             detail_id = visit[col_to_idx[self.id_detail_col]]
             visit_id = visit[col_to_idx[self.id_visit_col]]
             date = visit[col_to_idx[self.detail_date_col]]
             condition = pd.DataFrame(
                 {
                     self.id_detail_col: [detail_id] * n_condition,
                     self.id_visit_col: [visit_id] * n_condition,
@@ -372,20 +387,20 @@
             )
             condition_occurrence.append(condition)
 
         condition_occurrence = pd.concat(condition_occurrence).reset_index(drop=True)
         condition_occurrence[self.id_condition_col] = range(
             condition_occurrence.shape[0]
         )
-        condition_occurrence = add_other_columns(
-            condition_occurrence, self.other_condition_columns
+        return add_other_columns(
+            generator=self.generator,
+            table=condition_occurrence,
+            other_columns=self.other_condition_columns,
         )
 
-        return condition_occurrence
-
     def _generate_note(
         self,
         hospital_ids,
         visit_occurrence,
         note_types: Tuple[str] = ("CRH", "URGENCE", "ORDONNANCE"),
     ):
         date_col = self.date_col
@@ -400,32 +415,35 @@
                 visit_occurrence.care_site_id == care_site_id
             ].reset_index(drop=True)
             visit_care_site[date_col] = (
                 visit_care_site[date_col].view("int64") // 10**9
             )
             t0_visit = visit_care_site["t_0_min"].max()
             params = dict(
+                generator=self.generator,
                 care_site_id=care_site_id,
                 date_col=date_col,
                 note_date_col=note_date_col,
                 id_visit_col=id_visit_col,
                 note_type_col=note_type_col,
                 t0_visit=t0_visit,
                 mode=self.mode,
             )
             for note_type in note_types:
                 params["note_type"] = note_type
-                note = generate_note(visit_care_site, **params)
+                note = generate_note(visit_care_site=visit_care_site, **params)
                 notes.append(note)
 
         notes = pd.concat(notes).reset_index(drop=True)
         notes[id_note_col] = range(notes.shape[0])
-        notes = add_other_columns(notes, self.other_note_columns)
-
-        return notes
+        return add_other_columns(
+            generator=self.generator,
+            table=notes,
+            other_columns=self.other_note_columns,
+        )
 
     def _generate_concept(
         self, n_entity: int = 5, units: List[str] = ["g", "g/l", "mol", "s"]
     ):
         loinc_concept_id = []
         loinc_itm_concept_id = []
         loinc_concept_code = []
@@ -440,58 +458,58 @@
         anabio_concept_name = []
         anabio_itm_concept_name = []
         src_concept_name = []
         concept_id_1 = []
         concept_id_2 = []
         relationship_id = []
         for i in range(n_entity):
-            n_loinc = np.random.randint(1, 4)
+            n_loinc = self.generator.integers(1, 4)
             loinc_codes = [str(i) + str(j) + "-0" for j in range(n_loinc)]
             loinc_concept_code.extend(loinc_codes)
             loinc_concept_id.extend(loinc_codes)
-            unit_values = np.random.choice(units, n_loinc)
+            unit_values = self.generator.choice(units, n_loinc)
             for loinc_code in loinc_codes:
-                unit_value = np.random.choice(unit_values)
+                unit_value = self.generator.choice(unit_values)
                 loinc_concept_name.append("LOINC_" + loinc_code + "_" + unit_value)
-                has_loinc_itm = np.random.random() >= 0.5
+                has_loinc_itm = self.generator.random() >= 0.5
                 if has_loinc_itm:
                     loinc_id_itm = loinc_code + "_ITM"
                     loinc_itm_concept_code.append(loinc_code)
                     loinc_itm_concept_id.append(loinc_id_itm)
                     loinc_itm_concept_name.append(
                         "LOINC_" + loinc_id_itm + "_" + unit_value
                     )
-                n_anabio = np.random.randint(1, 3)
+                n_anabio = self.generator.integers(1, 3)
                 supp_code = "9" if len(str(i)) == 1 else ""
                 anabio_codes = [
                     "A" + loinc_code.split("-")[0] + str(j) + supp_code
                     for j in range(n_anabio)
                 ]
                 anabio_concept_code.extend(anabio_codes)
                 anabio_concept_id.extend(anabio_codes)
                 for anabio_code in anabio_codes:
                     anabio_concept_name.append(
                         "ANABIO_" + anabio_code + "_" + unit_value
                     )
-                    has_anabio_itm = np.random.random() >= 0.5
+                    has_anabio_itm = self.generator.random() >= 0.5
                     if has_anabio_itm:
                         anabio_id_itm = anabio_code + "_ITM"
                         anabio_itm_concept_code.append(anabio_code)
                         anabio_itm_concept_id.append(anabio_id_itm)
                         anabio_itm_concept_name.append(
                             "ANABIO_" + anabio_id_itm + "_" + unit_value
                         )
                         concept_id_1.extend([anabio_id_itm, anabio_code])
                         concept_id_2.extend([anabio_code, anabio_id_itm])
                         relationship_id.extend(["Maps to", "Mapped from"])
                         if has_loinc_itm:
                             concept_id_1.extend([anabio_id_itm, loinc_id_itm])
                             concept_id_2.extend([loinc_id_itm, anabio_id_itm])
                             relationship_id.extend(["Maps to", "Mapped from"])
-                    n_src = np.random.randint(1, 3)
+                    n_src = self.generator.integers(1, 3)
                     src_codes = [
                         loinc_code + "-" + anabio_code + "-" + str(j)
                         for j in range(n_src)
                     ]
                     src_concept_code.extend(src_codes)
                     src_concept_name.extend(
                         ["SRC_" + src_code + "_" + unit_value for src_code in src_codes]
@@ -575,30 +593,31 @@
         visit_occurrence = visit_occurrence.sample(frac=0.9)
         for concept_name in src_concept_name:
             concept_code = concept_name.split("_")[1]
             unit = concept_name.split("_")[-1]
             mean_value = (1 + units.index(unit)) * 2
             std_value = 1
             for care_site_id in hospital_ids:
-                t_start = t_min + np.random.randint(0, (t_max - t_min) / 20)
-                t_end = t_max - np.random.randint(0, (t_max - t_min) / 20)
+                t_start = t_min + self.generator.integers(0, (t_max - t_min) / 20)
+                t_end = t_max - self.generator.integers(0, (t_max - t_min) / 20)
                 valid_measurements = int(
-                    np.random.normal(mean_measurement, mean_measurement / 5)
+                    self.generator.normal(mean_measurement, mean_measurement / 5)
                 )
-                missing_value = int(np.random.uniform(1, valid_measurements / 10))
+                missing_value = int(self.generator.uniform(1, valid_measurements / 10))
                 n_measurements = valid_measurements + missing_value
-                increase_time = np.random.randint(
+                increase_time = self.generator.integers(
                     (t_end - t_start) / 100, (t_end - t_start) / 10
                 )
-                increase_ratio = np.random.uniform(150, 200)
+                increase_ratio = self.generator.uniform(150, 200)
                 concept_code = concept_name.split("_")[1]
                 unit = concept_name.split("_")[-1]
                 mean_value = (1 + units.index(unit)) * 2
                 std_value = 1
                 params = dict(
+                    generator=self.generator,
                     t_start=t_start,
                     t_end=t_end,
                     n_events=n_measurements,
                     increase_ratio=increase_ratio,
                     increase_time=increase_time,
                     bio_date_col=self.bio_date_col,
                     unit=unit,
@@ -611,30 +630,32 @@
                 ]
                 measurement[self.id_visit_col] = (
                     visit_care_site[self.id_visit_col]
                     .sample(n=measurement.shape[0], replace=True)
                     .reset_index(drop=True)
                 )
                 measurement["value_as_number"] = [None] * missing_value + list(
-                    np.random.normal(
+                    self.generator.normal(
                         mean_value, std_value, measurement.shape[0] - missing_value
                     )
                 )
                 measurements.append(measurement)
 
         measurements = pd.concat(measurements).reset_index(drop=True)
         measurements["value_source_value"] = (
             measurements["value_as_number"].astype(str)
             + " "
             + measurements["unit_source_value"].astype(str)
         )
         measurements[self.id_bio_col] = range(measurements.shape[0])
-        measurements = add_other_columns(measurements, self.other_measurement_columns)
-
-        return measurements
+        return add_other_columns(
+            generator=self.generator,
+            table=measurements,
+            other_columns=self.other_measurement_columns,
+        )
 
     def convert_to_koalas(self):
         if isinstance(self.care_site, ks.frame.DataFrame):
             logger.info("Module is already Koalas!")
             return
         self.care_site = ks.DataFrame(self.care_site)
         self.visit_occurrence = ks.DataFrame(self.visit_occurrence)
```

### Comparing `edsteva-0.2.0/edsteva/io/synthetic/utils.py` & `edsteva-0.2.1/edsteva/io/synthetic/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 
 
 def generate_events_before_t0(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     t0: int,
     increase_time: int,
     increase_ratio: float,
 ):
@@ -14,20 +15,21 @@
     n_before = int(
         (t0_before - t_start)
         * n_events
         / ((t0 - t_start) + increase_ratio * (t_end - t0))
     )
 
     return pd.to_datetime(
-        pd.Series(np.random.randint(t_start, t0_before, n_before)),
+        pd.Series(generator.integers(t_start, t0_before, n_before)),
         unit="s",
     )
 
 
 def generate_events_after_t0(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     t0: int,
     increase_time: int,
     increase_ratio: float,
 ):
@@ -36,20 +38,21 @@
         increase_ratio
         * (t_end - t0_after)
         * n_events
         / ((t0 - t_start) + increase_ratio * (t_end - t0))
     )
 
     return pd.to_datetime(
-        pd.Series(np.random.randint(t0_after, t_end, n_after)),
+        pd.Series(generator.integers(t0_after, t_end, n_after)),
         unit="s",
     )
 
 
 def generate_events_around_t0(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     t0: int,
     increase_time: int,
     increase_ratio: float,
 ):
@@ -60,23 +63,24 @@
         * (increase_ratio + 1)
         * n_events
         / ((t0 - t_start) + increase_ratio * (t_end - t0))
     )
 
     return pd.to_datetime(
         pd.Series(
-            np.random.triangular(
+            generator.triangular(
                 left=t0_before, right=t0_after, mode=t0_after, size=n_middle
             )
         ),
         unit="s",
     )
 
 
 def generate_events_around_t1(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     t1: int,
     increase_time: int,
     increase_ratio: float,
 ):
@@ -87,37 +91,38 @@
         * (increase_ratio + 1)
         * n_events
         / ((t1 - t_start) * increase_ratio + (t_end - t1))
     )
 
     return pd.to_datetime(
         pd.Series(
-            np.random.triangular(
+            generator.triangular(
                 left=t1_before, right=t1_after, mode=t1_before, size=n_middle
             )
         ),
         unit="s",
     )
 
 
 def generate_events_after_t1(
+    generator: np.random.Generator,
     t_start: int,
     t_end: int,
     n_events: int,
     t1: int,
     increase_time: int,
     increase_ratio: float,
 ):
     t1_after = t1 + increase_time / 2
     n_after = int(
         (t_end - t1_after) * n_events / ((t1 - t_start) * increase_ratio + (t_end - t1))
     )
 
     return pd.to_datetime(
-        pd.Series(np.random.randint(t1_after, t_end, n_after)),
+        pd.Series(generator.integers(t1_after, t_end, n_after)),
         unit="s",
     )
 
 
 def recursive_items(dictionary):
     for key, value in dictionary.items():
         if type(value) is dict:
```

### Comparing `edsteva-0.2.0/edsteva/metrics/error.py` & `edsteva-0.2.1/edsteva/metrics/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     | :----------------------- | :----------- | :----------- | :---- |
     | Unité Fonctionnelle (UF) | 8312056386   | 'Urg_Hospit' | 0.040 |
     | Unité Fonctionnelle (UF) | 8312056386   | 'All'        | 0.028 |
     | Pôle/DMU                 | 8312027648   | 'Urg_Hospit' | 0.022 |
     | Pôle/DMU                 | 8312027648   | 'All'        | 0.014 |
     | Hôpital                  | 8312022130   | 'Urg_Hospit' | 0.027 |
     """
-    check_columns(df=estimates, required_columns=index + [y_0])
-    check_columns(df=predictor, required_columns=index + [x, y])
+    check_columns(df=estimates, required_columns=[*index, y_0])
+    check_columns(df=predictor, required_columns=[*index, x, y])
 
     fitted_predictor = predictor.merge(estimates, on=index)
 
     fitted_predictor["loss"] = loss_function(
         fitted_predictor[y] - fitted_predictor[y_0]
     )
```

### Comparing `edsteva-0.2.0/edsteva/metrics/error_after_t0.py` & `edsteva-0.2.1/edsteva/metrics/error_after_t0.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,16 @@
     | :----------------------- | :----------- | :---------| :---- |
     | Unité Fonctionnelle (UF) | 8312056386   | 'Urg'     | 0.040 |
     | Unité Fonctionnelle (UF) | 8312056386   | 'All'     | 0.028 |
     | Pôle/DMU                 | 8312027648   | 'Urg'     | 0.022 |
     | Pôle/DMU                 | 8312027648   | 'All'     | 0.014 |
     | Hôpital                  | 8312022130   | 'Urg'     | 0.027 |
     """
-    check_columns(df=estimates, required_columns=index + [y_0, threshold])
-    check_columns(df=predictor, required_columns=index + [x, y])
+    check_columns(df=estimates, required_columns=[*index, y_0, threshold])
+    check_columns(df=predictor, required_columns=[*index, x, y])
 
     fitted_predictor = predictor.merge(estimates, on=index)
 
     fitted_predictor = fitted_predictor.dropna(subset=[threshold])
 
     fitted_predictor["loss"] = loss_function(
         fitted_predictor[y] - fitted_predictor[y_0]
```

### Comparing `edsteva-0.2.0/edsteva/metrics/error_between_t0_t1.py` & `edsteva-0.2.1/edsteva/metrics/error_between_t0_t1.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,16 +56,16 @@
     | :----------------------- | :----------- | :---------| :---- |
     | Unité Fonctionnelle (UF) | 8312056386   | 'Urg'     | 0.040 |
     | Unité Fonctionnelle (UF) | 8312056386   | 'All'     | 0.028 |
     | Pôle/DMU                 | 8312027648   | 'Urg'     | 0.022 |
     | Pôle/DMU                 | 8312027648   | 'All'     | 0.014 |
     | Hôpital                  | 8312022130   | 'Urg'     | 0.027 |
     """
-    check_columns(df=estimates, required_columns=index + [y_0, t_0, t_1])
-    check_columns(df=predictor, required_columns=index + [x, y])
+    check_columns(df=estimates, required_columns=[*index, y_0, t_0, t_1])
+    check_columns(df=predictor, required_columns=[*index, x, y])
 
     fitted_predictor = predictor.merge(estimates, on=index)
 
     fitted_predictor = fitted_predictor.dropna(subset=[t_0, t_1])
 
     fitted_predictor["loss"] = loss_function(
         fitted_predictor[y] - fitted_predictor[y_0]
```

### Comparing `edsteva-0.2.0/edsteva/models/base.py` & `edsteva-0.2.1/edsteva/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,16 +205,15 @@
         | Hôpital                  | 8312022130   | 'Urg_Hospit' | 2022-02-01 | 9746.0  | 0.974 | 0.912 |
 
         """
 
         predictor = probe.predictor
         index = probe._index
 
-        prediction = self.predict_process(predictor=predictor, index=index)
-        return prediction
+        return self.predict_process(predictor=predictor, index=index)
 
     def load(self, path=None) -> None:
         """Loads a Model from local
 
         Parameters
         ----------
         path : str, optional
@@ -310,19 +309,15 @@
         metrics_df = []
         for metric_function in metric_functions:
             metrics_df.append(
                 metrics.get(metric_function)(
                     predictor=predictor, estimates=estimates, index=index
                 )
             )
-        metrics_df = reduce(
-            lambda left, right: pd.merge(left, right, on=index), metrics_df
-        )
-
-        return metrics_df
+        return reduce(lambda left, right: left.merge(right, on=index), metrics_df)
 
     def is_predictable_probe(
         self,
         predictor: pd.DataFrame,
         index: List[str],
     ) -> pd.DataFrame:
         """Raises an error if the model has not been fitted on the input predictor.
@@ -344,14 +339,12 @@
         Exception
             Some indexes have no associated estimates, the model must be fitted on an adequate probe
         """
         prediction = predictor.merge(
             self.estimates, on=index, how="left", validate="many_to_one", indicator=True
         )
         if (prediction["_merge"] == "both").all():
-            prediction = prediction.drop(columns="_merge")
-            return prediction
+            return prediction.drop(columns="_merge")
 
-        else:
-            raise Exception(
-                "Some indexes have no associated estimates, the model must be fitted on an adequate probe"
-            )
+        raise Exception(
+            "Some indexes have no associated estimates, the model must be fitted on an adequate probe"
+        )
```

### Comparing `edsteva-0.2.0/edsteva/models/rectangle_function/algos/loss_minimization.py` & `edsteva-0.2.1/edsteva/models/rectangle_function/algos/loss_minimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     y_col : str, optional
         Column name  for the completeness variable $c(t)$.
     loss_function : Callable, optional
         The loss function $\mathcal{L}$.
     min_rect_month_width : int, optional
         Min number of months between $t_0$ and $t_1$.
     """
-    check_columns(df=predictor, required_columns=index + [x_col, y_col])
+    check_columns(df=predictor, required_columns=[*index, x_col, y_col])
     predictor = predictor.sort_values(x_col)
-    cols = index + [x_col, y_col]
+    cols = [*index, x_col, y_col]
     iter = predictor[cols].groupby(index)
     results = []
     for partition, group in iter:
         row = dict(zip(index, partition))
         t_0, c_0, t_1 = _compute_one_double_threshold(
             group,
             x_col,
@@ -76,15 +76,15 @@
 def _compute_one_double_threshold(
     group: pd.DataFrame,
     x_col: str,
     y_col: str,
     loss_func: Callable,
     min_rect_month_width: int,
 ):
-    target = group[[x_col, y_col]].values
+    target = group[[x_col, y_col]].to_numpy()
     best_x0 = best_y0 = best_x1 = None
     best_loss = np.inf
     for idx in range(len(target) - min_rect_month_width):
         x0 = target[idx, 0]
         y_before_x0 = target[:idx, 1]
         for jdx in range(idx + min_rect_month_width, len(target)):
             x1 = target[jdx, 0]
```

### Comparing `edsteva-0.2.0/edsteva/models/rectangle_function/rectangle_function.py` & `edsteva-0.2.1/edsteva/models/rectangle_function/rectangle_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,15 @@
         ----------
         predictor : pd.DataFrame
             Target variable to be fitted
         index : List[str], optional
             Variable from which data is grouped
             **EXAMPLE**: `["care_site_level", "stay_type", "note_type", "care_site_id"]`
         """
-        estimates = algos.get(self._algo)(predictor=predictor, index=index, **kwargs)
-
-        return estimates
+        return algos.get(self._algo)(predictor=predictor, index=index, **kwargs)
 
     def predict_process(
         self,
         predictor: pd.DataFrame,
         index: List[str],
     ):
         """Script to be used by [``predict()``][edsteva.models.base.BaseModel.predict]
```

### Comparing `edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/__init__.py` & `edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/defaults.py` & `edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py` & `edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def get_normalized_probe_dashboard_config(self, predictor: DataFrame):
     c_0_min_selection, c_0_min_filter = get_c_0_min_selection(predictor=predictor)
     t_0_selection, t_0_min_filter = get_t_0_selection(predictor=predictor)
     t_1_selection, t_1_min_filter = get_t_1_selection(predictor=predictor)
     error_max_selection, error_max_filter = get_error_max_selection(predictor=predictor)
-    normalized_probe_plot_config = dict(
+    return dict(
         estimates_selections=[
             t_0_selection,
             t_1_selection,
             c_0_min_selection,
             error_max_selection,
         ],
         estimates_filters=[
@@ -31,8 +31,7 @@
             error_max_filter,
         ],
         probe_line=normalized_probe_line,
         model_line=normalized_model_line,
         extra_horizontal_bar_charts=[horizontal_min_c0, horizontal_max_error],
         extra_vertical_bar_charts=[],
     )
-    return normalized_probe_plot_config
```

### Comparing `edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py` & `edsteva-0.2.1/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def get_normalized_probe_plot_config(self, predictor: DataFrame):
     c_0_min_selection, c_0_min_filter = get_c_0_min_selection(predictor=predictor)
     t_0_selection, t_0_min_filter = get_t_0_selection(predictor=predictor)
     t_1_selection, t_1_min_filter = get_t_1_selection(predictor=predictor)
     error_max_selection, error_max_filter = get_error_max_selection(predictor=predictor)
-    normalized_probe_dashboard_config = dict(
+    return dict(
         estimates_selections=[
             t_0_selection,
             t_1_selection,
             c_0_min_selection,
             error_max_selection,
         ],
         estimates_filters=[
@@ -27,8 +27,7 @@
             t_1_min_filter,
             c_0_min_filter,
             error_max_filter,
         ],
         probe_line=normalized_probe_line,
         model_line=normalized_model_line,
     )
-    return normalized_probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/models/step_function/algos/loss_minimization.py` & `edsteva-0.2.1/edsteva/models/step_function/algos/loss_minimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     x_col : str, optional
         Column name for the time variable $t$
     y_col : str, optional
         Column name  for the completeness variable $c(t)$
     loss_function : Callable, optional
         The loss function $\mathcal{L}$
     """
-    check_columns(df=predictor, required_columns=index + [x_col, y_col])
+    check_columns(df=predictor, required_columns=[*index, x_col, y_col])
     predictor = predictor.sort_values(x_col)
-    cols = index + [x_col, y_col]
+    cols = [*index, x_col, y_col]
     iter = predictor[cols].groupby(index)
     results = []
     for partition, group in iter:
         row = dict(zip(index, partition))
         t_0, c_0 = _compute_one_threshold(
             group,
             x_col,
@@ -70,15 +70,15 @@
 
 def _compute_one_threshold(
     group: pd.DataFrame,
     x_col: str,
     y_col: str,
     loss_func: Callable,
 ):
-    target = group[[x_col, y_col]].values
+    target = group[[x_col, y_col]].to_numpy()
     best_loss, best_x0, best_y0 = np.inf, None, None
     for idx in range(len(target)):
         x0 = target[idx, 0]
         y_before_x0 = target[:idx, 1]
         y_after_x0 = target[idx:, 1]
         y0 = y_after_x0.mean()
         residual = np.hstack([y_before_x0, (y_after_x0 - y0)])
```

### Comparing `edsteva-0.2.0/edsteva/models/step_function/algos/quantile.py` & `edsteva-0.2.1/edsteva/models/step_function/algos/quantile.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,15 @@
     index: List[str],
     q: float = 0.8,
     x: str = "date",
     y: str = "c",
     threshold: str = "c_0",
 ):
     estimates = c_0_from_quantile(predictor=predictor, index=index, q=q, x=x, y=y)
-    estimates = t_0_from_c_0(
-        predictor=estimates, index=index, x=x, y=y, threshold=threshold
-    )
-    return estimates
+    return t_0_from_c_0(predictor=estimates, index=index, x=x, y=y, threshold=threshold)
 
 
 def c_0_from_quantile(
     predictor: pd.DataFrame,
     index: List[str],
     q: float = 0.8,
     x: str = "date",
@@ -46,15 +43,15 @@
         Quantile value
     x : str, optional
         Column name for the time variable $t$
     y : str, optional
         Column name  for the completeness variable $c(t)$
     """
 
-    check_columns(df=predictor, required_columns=index + [x, y])
+    check_columns(df=predictor, required_columns=[*index, x, y])
 
     quantile = (
         predictor.groupby(index)[[y]]
         .agg(lambda g: np.quantile(g, q=q))
         .rename(columns={y: "c_0"})
     )
 
@@ -86,15 +83,15 @@
         Column name for the time variable $t$
     y : str, optional
         Column name  for the completeness variable $c(t)$
     threshold : str, optional
         Column name  for the threshold variable $t_0$
     """
 
-    check_columns(df=predictor, required_columns=index + [x, y, threshold])
+    check_columns(df=predictor, required_columns=[*index, x, y, threshold])
 
     threshold = (
         predictor[predictor[y] > predictor[threshold]]
         .groupby(index)[[x]]
         .min()
         .rename(columns={x: "t_0"})
     )
```

### Comparing `edsteva-0.2.0/edsteva/models/step_function/step_function.py` & `edsteva-0.2.1/edsteva/models/step_function/step_function.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/models/step_function/viz_configs/__init__.py` & `edsteva-0.2.1/edsteva/models/step_function/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/models/step_function/viz_configs/defaults.py` & `edsteva-0.2.1/edsteva/models/step_function/viz_configs/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py` & `edsteva-0.2.1/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 )
 
 
 def get_normalized_probe_dashboard_config(self, predictor: DataFrame):
     c_0_min_selection, c_0_min_filter = get_c_0_min_selection(predictor=predictor)
     t_0_selection, t_0_min_filter = get_t_0_selection(predictor=predictor)
     error_max_selection, error_max_filter = get_error_max_selection(predictor=predictor)
-    normalized_probe_plot_config = dict(
+    return dict(
         estimates_selections=[c_0_min_selection, t_0_selection, error_max_selection],
         estimates_filters=[c_0_min_filter, t_0_min_filter, error_max_filter],
         probe_line=normalized_probe_line,
         model_line=normalized_model_line,
         extra_horizontal_bar_charts=[horizontal_min_c0, horizontal_max_error],
         extra_vertical_bar_charts=[],
     )
-    return normalized_probe_plot_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/base.py` & `edsteva-0.2.1/edsteva/probes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 from abc import ABCMeta, abstractmethod
-from typing import Dict, List, Union
+from typing import ClassVar, Dict, List, Union
 
 import pandas as pd
 from loguru import logger
 
 from edsteva import CACHE_DIR
 from edsteva.probes.utils.filter_df import filter_table_by_care_site
 from edsteva.probes.utils.prepare_df import prepare_care_site_relationship
@@ -30,15 +30,15 @@
         It is a copy of the predictor DataFrame used to [``reset_predictor()``][edsteva.probes.base.BaseProbe.reset_predictor]
     care_site_relationship: pd.DataFrame
         Available with the [``compute()``][edsteva.probes.base.BaseProbe.compute] method
 
         It describes the care site structure (cf. [``prepare_care_site_relationship()``][edsteva.probes.utils.prepare_df.prepare_care_site_relationship])
     """
 
-    _schema = ["care_site_level", "care_site_id", "date", "c"]
+    _schema: ClassVar[List[str]] = ["care_site_level", "care_site_id", "date", "c"]
 
     def __init__(
         self,
         completeness_predictor: str,
         index: List[str],
     ):
         self._completeness_predictor = completeness_predictor
@@ -79,25 +79,25 @@
                 raise Exception(
                     "Predictor is empty, please review the process method or your arguments"
                 )
             check_columns(
                 self.predictor,
                 required_columns=self._schema,
             )
-            if not self.predictor.dtypes["date"] == "datetime64[ns]":
+            if self.predictor.dtypes["date"] != "datetime64[ns]":
                 try:
                     self.predictor["date"] = self.predictor["date"].astype(
                         "datetime64[ns]"
                     )
                 except Exception as e:
                     raise TypeError(
                         "Predictor column 'date' type is {} and cannot convert to datetime and return the following error: {}. Please review the process method or your arguments".format(
                             self.predictor.dtypes["date"], e
                         )
-                    )
+                    ) from e
         else:
             raise Exception(
                 "Predictor has not been computed, please use the compute method as follow: Predictor.compute()"
             )
 
     def filter_date_per_care_site(self, target_column: str):
         filtered_predictor = self.predictor.copy()
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/biology.py` & `edsteva-0.2.1/edsteva/probes/biology/biology.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/per_measurement.py` & `edsteva-0.2.1/edsteva/probes/biology/completeness_predictors/per_measurement.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     return compute_completeness(self, biology_predictor)
 
 
 def compute_completeness(
     self,
     biology_predictor: DataFrame,
 ):
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
     n_measurement = (
         biology_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"measurement_id": "nunique"})
@@ -157,17 +157,15 @@
         on=partition_cols,
     )
 
     biology_predictor["c"] = biology_predictor["max_n_measurement"].where(
         biology_predictor["max_n_measurement"] == 0,
         biology_predictor["n_measurement"] / biology_predictor["max_n_measurement"],
     )
-    biology_predictor = biology_predictor.drop(columns="max_n_measurement")
-
-    return biology_predictor
+    return biology_predictor.drop(columns="max_n_measurement")
 
 
 def get_hospital_measurements(
     measurement: DataFrame,
     visit_occurrence: DataFrame,
     care_site: DataFrame,
 ):
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/per_visit.py` & `edsteva-0.2.1/edsteva/probes/biology/completeness_predictors/per_visit.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 
 def compute_completeness(
     self,
     biology_predictor: DataFrame,
 ):
     # Visit with measurement
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
     n_visit_with_measurement = (
         biology_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"has_measurement": "count"})
@@ -183,15 +183,15 @@
     self,
     measurement: DataFrame,
     visit_occurrence: DataFrame,
     care_site: DataFrame,
 ):
     hospital_measurement = measurement[
         set(measurement.columns).intersection(
-            set(["visit_occurrence_id"] + self._index)
+            set(["visit_occurrence_id", *self._index])
         )
     ].drop_duplicates()
     hospital_measurement["has_measurement"] = True
     hospital_visit = visit_occurrence.merge(
         hospital_measurement,
         on="visit_occurrence_id",
         how="left",
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/__init__.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/defaults.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 )
 
 
 def get_normalized_probe_dashboard_config(self):
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
-    normalized_probe_dashboard_config = dict(
+    return dict(
         chart_style=chart_style,
         main_chart=normalized_main_chart,
         time_line=normalized_time_line,
         error_line=error_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
-
-    return normalized_probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 
 
 def get_probe_dashboard_config(self):
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
-    probe_dashboard_config = dict(
+    return dict(
         chart_style=chart_style,
         main_chart=main_chart,
         time_line=time_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
-    return probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/defaults.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 )
 
 
 def get_normalized_probe_dashboard_config(self):
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
-    normalized_probe_dashboard_config = dict(
+    return dict(
         chart_style=chart_style,
         main_chart=normalized_main_chart,
         time_line=normalized_time_line,
         error_line=error_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
-
-    return normalized_probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 
 
 def get_probe_dashboard_config(self):
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
-    probe_dashboard_config = dict(
+    return dict(
         chart_style=chart_style,
         main_chart=main_chart,
         time_line=time_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
-    return probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/defaults.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 )
 
 
 def get_normalized_probe_dashboard_config(self):
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
-    normalized_probe_dashboard_config = dict(
+    return dict(
         chart_style=chart_style,
         main_chart=normalized_main_chart,
         time_line=normalized_time_line,
         error_line=error_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
-
-    return normalized_probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py` & `edsteva-0.2.1/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 
 
 def get_probe_dashboard_config(self):
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
-    probe_dashboard_config = dict(
+    return dict(
         chart_style=chart_style,
         main_chart=main_chart,
         time_line=time_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
-    return probe_dashboard_config
```

### Comparing `edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_condition.py` & `edsteva-0.2.1/edsteva/probes/condition/completeness_predictors/per_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     return compute_completeness(self, condition_predictor)
 
 
 def compute_completeness(
     self,
     condition_predictor: DataFrame,
 ):
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
 
     n_condition = (
         condition_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
@@ -166,17 +166,15 @@
         on=partition_cols,
     )
 
     condition_predictor["c"] = condition_predictor["max_n_condition"].where(
         condition_predictor["max_n_condition"] == 0,
         condition_predictor["n_condition"] / condition_predictor["max_n_condition"],
     )
-    condition_predictor = condition_predictor.drop(columns="max_n_condition")
-
-    return condition_predictor
+    return condition_predictor.drop(columns="max_n_condition")
 
 
 def get_hospital_condition(
     condition_occurrence: DataFrame,
     visit_occurrence: DataFrame,
     care_site: DataFrame,
 ):
```

### Comparing `edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_visit.py` & `edsteva-0.2.1/edsteva/probes/condition/completeness_predictors/per_visit.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 
 def compute_completeness(
     self,
     condition_predictor: DataFrame,
 ):
     # Visit with diagnosis
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
     n_visit_with_condition = (
         condition_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"has_condition": "count"})
```

### Comparing `edsteva-0.2.0/edsteva/probes/condition/condition.py` & `edsteva-0.2.1/edsteva/probes/condition/condition.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/condition/viz_configs/__init__.py` & `edsteva-0.2.1/edsteva/probes/condition/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/defaults.py` & `edsteva-0.2.1/edsteva/probes/condition/viz_configs/n_condition/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/defaults.py` & `edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_condition/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/defaults.py` & `edsteva-0.2.1/edsteva/probes/condition/viz_configs/per_visit/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_note.py` & `edsteva-0.2.1/edsteva/probes/note/completeness_predictors/per_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     return compute_completeness(self, note_predictor)
 
 
 def compute_completeness(
     self,
     note_predictor: DataFrame,
 ):
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
 
     n_note = (
         note_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
@@ -154,17 +154,15 @@
         on=partition_cols,
     )
 
     note_predictor["c"] = note_predictor["max_n_note"].where(
         note_predictor["max_n_note"] == 0,
         note_predictor["n_note"] / note_predictor["max_n_note"],
     )
-    note_predictor = note_predictor.drop(columns="max_n_note")
-
-    return note_predictor
+    return note_predictor.drop(columns="max_n_note")
 
 
 def get_hospital_note(
     note: DataFrame,
     visit_occurrence: DataFrame,
     care_site: DataFrame,
 ):
```

### Comparing `edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_visit.py` & `edsteva-0.2.1/edsteva/probes/note/completeness_predictors/per_visit.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 
 def compute_completeness(
     self,
     note_predictor: DataFrame,
 ):
     # Visit with note
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
     n_visit_with_note = (
         note_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"has_note": "count"})
```

### Comparing `edsteva-0.2.0/edsteva/probes/note/note.py` & `edsteva-0.2.1/edsteva/probes/note/note.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/note/viz_configs/__init__.py` & `edsteva-0.2.1/edsteva/probes/note/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/defaults.py` & `edsteva-0.2.1/edsteva/probes/note/viz_configs/n_note/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/defaults.py` & `edsteva-0.2.1/edsteva/probes/note/viz_configs/per_note/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/defaults.py` & `edsteva-0.2.1/edsteva/probes/note/viz_configs/per_visit/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/utils/filter_df.py` & `edsteva-0.2.1/edsteva/probes/utils/filter_df.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/utils/prepare_df.py` & `edsteva-0.2.1/edsteva/probes/utils/prepare_df.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,17 +404,15 @@
     ]
 
     note_ref = note_ref.melt(
         id_vars="note_id",
         value_name="care_site_source_value",
     )
     note_ref = note_ref.merge(care_site_ref, on="care_site_source_value")
-    note = note.merge(note_ref[["note_id", "care_site_id"]], on="note_id")
-
-    return note
+    return note.merge(note_ref[["note_id", "care_site_id"]], on="note_id")
 
 
 def prepare_visit_detail(
     data: Data,
     start_date: datetime,
     end_date: datetime,
 ):
@@ -435,23 +433,21 @@
             "visit_detail_type_source_value": "visit_detail_type",
         }
     )
     visit_detail = filter_valid_observations(
         table=visit_detail, table_name="visit_detail", valid_naming="Actif"
     )
 
-    visit_detail = filter_table_by_date(
+    return filter_table_by_date(
         table=visit_detail,
         table_name="visit_detail",
         start_date=start_date,
         end_date=end_date,
     )
 
-    return visit_detail
-
 
 def prepare_care_site_relationship(data: Data) -> pd.DataFrame:
     """Computes hierarchical care site structure
 
     Parameters
     ----------
     data : Data
```

### Comparing `edsteva-0.2.0/edsteva/probes/utils/utils.py` & `edsteva-0.2.1/edsteva/probes/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,19 @@
 
     # Generate all available partitions
     all_partitions = (
         predictor[list(set(partition_cols) - {"date"})]
         .drop_duplicates()
         .merge(date_index, how="cross")
     )
-    filled_predictor = all_partitions.merge(
+    return all_partitions.merge(
         predictor,
         on=partition_cols,
         how="left",
     ).fillna({col: 0 for col in set(predictor.columns) - set(partition_cols)})
-    return filled_predictor
 
 
 def hospital_only(care_site_levels: List[str]):
     if not isinstance(care_site_levels, list):
         care_site_levels = [care_site_levels]
     return len(care_site_levels) == 1 and (
         care_site_levels[0] == "Hospital"
@@ -201,11 +200,8 @@
             columns={
                 "child_care_site_id": "care_site_id",
                 "child_care_site_level": "care_site_level",
                 "child_care_site_specialty": "care_site_specialty",
             }
         )
 
-    extended_care_site_id_to_filter = pd.concat(
-        extended_care_site_id_to_filter
-    ).drop_duplicates()
-    return extended_care_site_id_to_filter
+    return pd.concat(extended_care_site_id_to_filter).drop_duplicates()
```

### Comparing `edsteva-0.2.0/edsteva/probes/visit/completeness_predictors/per_visit.py` & `edsteva-0.2.1/edsteva/probes/visit/completeness_predictors/per_visit.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     return compute_completeness(self, visit_predictor)
 
 
 def compute_completeness(
     self,
     visit_predictor: DataFrame,
 ):
-    partition_cols = self._index.copy() + ["date"]
+    partition_cols = [*self._index.copy(), "date"]
 
     n_visit = (
         visit_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
@@ -154,17 +154,15 @@
         on=partition_cols,
     )
 
     visit_predictor["c"] = visit_predictor["max_n_visit"].where(
         visit_predictor["max_n_visit"] == 0,
         visit_predictor["n_visit"] / visit_predictor["max_n_visit"],
     )
-    visit_predictor = visit_predictor.drop(columns="max_n_visit")
-
-    return visit_predictor
+    return visit_predictor.drop(columns="max_n_visit")
 
 
 def get_hospital_visit(
     visit_occurrence: DataFrame,
     care_site: DataFrame,
 ):
     hospital_visit = visit_occurrence.rename(
```

### Comparing `edsteva-0.2.0/edsteva/probes/visit/visit.py` & `edsteva-0.2.1/edsteva/probes/visit/visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/visit/viz_configs/__init__.py` & `edsteva-0.2.1/edsteva/probes/visit/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/defaults.py` & `edsteva-0.2.1/edsteva/probes/visit/viz_configs/n_visit/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/defaults.py` & `edsteva-0.2.1/edsteva/probes/visit/viz_configs/per_visit/defaults.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/utils/checks.py` & `edsteva-0.2.1/edsteva/utils/checks.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/utils/file_management.py` & `edsteva-0.2.1/edsteva/utils/file_management.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-import os
 from pathlib import Path
 
 import _pickle as pickle
 from loguru import logger
 
 
 def save_object(obj, filename: Path):
     if not isinstance(filename, Path):
         filename = Path(filename)
-    os.makedirs(filename.parent, exist_ok=True)
-    with open(filename, "wb") as outp:  # Overwrites any existing file.
+    Path.mkdir(filename.parent, exist_ok=True, parents=True)
+    with Path.open(filename, "wb") as outp:  # Overwrites any existing file.
         pickle.dump(obj, outp, -1)
         logger.info("Saved to {}", filename)
 
 
 def load_object(filename: str):
-    if os.path.isfile(filename):
-        with open(filename, "rb") as obj:
+    file = Path(filename)
+    if Path.is_file(file):
+        with Path.open(file, "rb") as obj:
             logger.info("Successfully loaded from {}", filename)
             return pickle.load(obj)
     else:
         raise FileNotFoundError(
             "There is no file found in {}".format(
                 filename,
             )
         )
 
 
 def delete_object(obj, filename: str):
-    if os.path.isfile(filename):
-        os.remove(filename)
+    file = Path(filename)
+    if Path.is_file(file):
+        Path.unlink(file)
         logger.info(
             "Removed from {}",
             filename,
         )
         if hasattr(obj, "path"):
             del obj.path
     else:
```

### Comparing `edsteva-0.2.0/edsteva/utils/framework.py` & `edsteva-0.2.1/edsteva/utils/framework.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,31 @@
 }
 
 
 def get_framework(obj: DataObject) -> Optional[ModuleType]:
     for _, framework in VALID_FRAMEWORKS.items():
         if obj.__class__.__module__.startswith(framework.__name__):
             return framework
-    # raise ValueError(f"Object from unknown framework: {obj}")
     return None
 
 
 def is_pandas(obj: DataObject) -> bool:
     return get_framework(obj) == _pandas
 
 
 def is_koalas(obj: DataObject) -> bool:
     return get_framework(obj) == _koalas
 
 
 def to(framework: str, obj: DataObject) -> DataObject:
     if framework == "koalas" or framework is _koalas:
         return koalas(obj)
-    elif framework == "pandas" or framework is _pandas:
+    if framework == "pandas" or framework is _pandas:
         return pandas(obj)
-    else:
-        raise ValueError(f"Unknown framework: {framework}")
+    raise ValueError(f"Unknown framework: {framework}")
 
 
 def pandas(obj: DataObject) -> DataObject:
     if get_framework(obj) is _pandas:
         return obj
 
     # Try using pyarrow via HDFS to convert object to pandas as it is way faster.
```

### Comparing `edsteva-0.2.0/edsteva/viz/dashboards/normalized_probe/normalized_probe.py` & `edsteva-0.2.1/edsteva/viz/dashboards/normalized_probe/normalized_probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/viz/dashboards/probe/fitted_probe.py` & `edsteva-0.2.1/edsteva/viz/dashboards/probe/fitted_probe.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,10 +120,8 @@
         main_chart = main_chart.add_params(index_selection)
     chart = concatenate_charts(
         main_chart=main_chart,
         time_line=time_line,
         horizontal_bar_charts=horizontal_bar_charts,
         vertical_bar_charts=vertical_bar_charts,
     )
-    chart = configure_style(chart=chart, chart_style=chart_style)
-
-    return chart
+    return configure_style(chart=chart, chart_style=chart_style)
```

### Comparing `edsteva-0.2.0/edsteva/viz/dashboards/probe/probe.py` & `edsteva-0.2.1/edsteva/viz/dashboards/probe/probe.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,10 +96,8 @@
         main_chart = main_chart.add_params(index_selection)
     chart = concatenate_charts(
         main_chart=main_chart,
         time_line=time_line,
         horizontal_bar_charts=horizontal_bar_charts,
         vertical_bar_charts=vertical_bar_charts,
     )
-    chart = configure_style(chart=chart, chart_style=chart_style)
-
-    return chart
+    return configure_style(chart=chart, chart_style=chart_style)
```

### Comparing `edsteva-0.2.0/edsteva/viz/dashboards/probe/wrapper.py` & `edsteva-0.2.1/edsteva/viz/dashboards/probe/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,15 @@
             horizontal_bar_charts_config["x"] = (
                 horizontal_bar_charts_config["x"]
                 + model_config["extra_horizontal_bar_charts"]
             )
     if not chart_style:
         chart_style = probe_config["chart_style"]
 
-    if fitted_model:
-        predictor = fitted_model.predict(probe)
-    else:
-        predictor = probe.predictor.copy()
+    predictor = fitted_model.predict(probe) if fitted_model else probe.predictor.copy()
     predictor = filter_predictor(
         predictor=predictor,
         care_site_level=care_site_level,
         **kwargs,
     )
 
     if fitted_model:
```

### Comparing `edsteva-0.2.0/edsteva/viz/plots/estimates_densities/estimates_densities.py` & `edsteva-0.2.1/edsteva/viz/plots/estimates_densities/estimates_densities.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         start_date=start_date,
         end_date=end_date,
         **kwargs,
     )
     estimates = fitted_model.estimates.copy()
     estimates = estimates.merge(
         predictor[
-            predictor.columns.intersection(set(probe._index + ["care_site_short_name"]))
+            predictor.columns.intersection(set([*probe._index, "care_site_short_name"]))
         ].drop_duplicates(),
         on=list(predictor.columns.intersection(set(probe._index))),
     )
     probe_config = deepcopy(probe.get_viz_config("estimates_densities_plot"))
     if not vertical_bar_charts_config:
         vertical_bar_charts_config = probe_config["vertical_bar_charts"]
     if not horizontal_bar_charts_config:
```

### Comparing `edsteva-0.2.0/edsteva/viz/plots/normalized_probe/normalized_probe.py` & `edsteva-0.2.1/edsteva/viz/plots/normalized_probe/normalized_probe.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     remove_care_site_id: bool, optional
         If False, it will display care site id and care site name, else only care site name.
     """
 
     predictor = probe.predictor.copy()
     estimates = fitted_model.estimates.copy()
 
-    cols_to_remove = ["date"] + probe._metrics
+    cols_to_remove = ["date", *probe._metrics]
     if remove_care_site_id:
         cols_to_remove.append("care_site_id")
     indexes = list(set(predictor.columns).difference(cols_to_remove))
     predictor = predictor.merge(estimates, on=probe._index)
 
     probe_config = deepcopy(probe.get_viz_config("normalized_probe_plot"))
     model_config = deepcopy(
```

### Comparing `edsteva-0.2.0/edsteva/viz/plots/probe/fitted_probe.py` & `edsteva-0.2.1/edsteva/viz/plots/probe/fitted_probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/viz/plots/probe/probe.py` & `edsteva-0.2.1/edsteva/viz/plots/probe/probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.0/edsteva/viz/plots/probe/wrapper.py` & `edsteva-0.2.1/edsteva/viz/plots/probe/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     probe_config = deepcopy(probe.get_viz_config("probe_plot"))
     if not main_chart_config:
         main_chart_config = probe_config["main_chart"]
     if not chart_style:
         chart_style = probe_config["chart_style"]
     predictor = probe.predictor.copy()
-    cols_to_remove = ["date"] + probe._metrics
+    cols_to_remove = ["date", *probe._metrics]
     if remove_care_site_id:
         cols_to_remove.append("care_site_id")
     indexes = list(set(predictor.columns).difference(cols_to_remove))
 
     if fitted_model:
         predictor = fitted_model.predict(probe).copy()
     else:
```

### Comparing `edsteva-0.2.0/edsteva/viz/utils.py` & `edsteva-0.2.1/edsteva/viz/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from datetime import datetime
 from functools import reduce
 from math import ceil, floor, log10
 from pathlib import Path
 from typing import Dict, List, Union
 
 import altair as alt
@@ -59,38 +58,33 @@
     if "calculates" in model_line_config.keys():
         for calculate in model_line_config["calculates"]:
             model_line = model_line.transform_calculate(**calculate)
     if "filters" in model_line_config.keys():
         for filter in model_line_config["filters"]:
             model_line = model_line.transform_filter(**filter)
     model_line = model_line.encode(**model_line_config["encode"])
-    model_line = add_selection_on_legend(model_line)
-    return model_line
+    return add_selection_on_legend(model_line)
 
 
 def generate_error_line(
     main_chart: alt.Chart,
     error_line_config: Dict[str, str],
 ):
     error_line = main_chart.mark_errorband(
         **error_line_config["mark_errorband"]
     ).encode(**error_line_config["encode"])
-    error_line = add_selection_on_legend(
-        error_line, opacity_true=0.3, opacity_false=0.05
-    )
-    return error_line
+    return add_selection_on_legend(error_line, opacity_true=0.3, opacity_false=0.05)
 
 
 def generate_probe_line(
     main_chart: alt.Chart,
     probe_line_config: Dict[str, str],
 ):
     probe_line = main_chart.mark_line().encode(**probe_line_config["encode"])
-    probe_line = add_selection_on_legend(probe_line)
-    return probe_line
+    return add_selection_on_legend(probe_line)
 
 
 def generate_time_line(
     base: alt.Chart,
     time_line_config: Dict[str, str],
 ):
     time_selection = alt.selection_interval(encodings=["x"])
@@ -201,20 +195,19 @@
     return base
 
 
 def add_selection_on_legend(
     chart: alt.Chart, opacity_true: float = 1, opacity_false: float = 0.2
 ):
     legend_selection = alt.selection_point(fields=["value"], bind="legend")
-    chart = chart.encode(
+    return chart.encode(
         opacity=alt.condition(
             legend_selection, alt.value(opacity_true), alt.value(opacity_false)
         )
     ).add_params(legend_selection)
-    return chart
 
 
 def add_estimates_filters(
     base: alt.Chart,
     estimates_filters: Dict[str, alt.SelectionParameter],
     selection_charts: Dict[str, List[alt.Chart]] = None,
 ):
@@ -364,36 +357,34 @@
     filename : str
         Folder path where to save the chart in HTML format.
 
         **EXAMPLE**: `"my_folder/my_file.html"`
     """
     if not isinstance(filename, Path):
         filename = Path(filename)
-    os.makedirs(filename.parent, exist_ok=True)
+    Path.mkdir(filename.parent, exist_ok=True, parents=True)
     if hasattr(obj, "save"):
         obj.save(filename)
     else:
-        with open(filename, "w") as f:
+        with Path.open(filename, "w") as f:
             f.write(obj)
     logger.info("The chart has been saved in {}", filename)
 
 
 def round_up(x: float, sig: int):
     if x == 0:
         return 0
-    else:
-        decimals = sig - floor(log10(abs(x))) - 1
-        return ceil(x * 10**decimals) / 10**decimals
+    decimals = sig - floor(log10(abs(x))) - 1
+    return ceil(x * 10**decimals) / 10**decimals
 
 
 def scale_it(x: float):
     if x == 0:
         return 1
-    else:
-        return 10 ** ceil(log10(x))
+    return 10 ** ceil(log10(x))
 
 
 def filter_predictor(
     predictor: pd.DataFrame,
     care_site_level: str = None,
     stay_type: List[str] = None,
     care_site_id: List[int] = None,
```

### Comparing `edsteva-0.2.0/pyproject.toml` & `edsteva-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edsteva"
-version = "0.2.0"
+version = "0.2.1"
 description = "EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records."
 authors = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Benoit Playe <benoit.playe@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>", "Paul Bernard <paul.bernard@aphp.fr>"]
 keywords = ["OMOP", "Data Analysis", "Electronic health record"]
 readme = "README.md"
 maintainers = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Thomas Petit-Jean <thomas.petitjean@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>"]
 homepage = "https://github.com/aphp/edsteva"
 repository = "https://github.com/aphp/edsteva"
@@ -45,15 +45,15 @@
 jupyterlab = "^3.0.0"
 
 [tool.poetry.group.docs.dependencies]
 pypandoc = "1.7.5"
 markdown = "^3.3.4"
 mkdocs-autorefs = "0.4.1"
 mkdocs-bibtex = "^2.0.1"
-mkdocs-charts-plugin = "0.0.8"
+mkdocs-charts-plugin = "0.0.9"
 mkdocs-gen-files = "0.3.5"
 mkdocs-img2fig-plugin = "0.9.3"
 mkdocs-literate-nav = "0.4.1"
 mkdocs-material = "^9.0.0"
 mkdocs-section-index = "0.3.4"
 black = "^23.1.0"
 termynal = "0.2.0"
@@ -61,22 +61,23 @@
 jinja2 = "~3.0.0"
 mkdocstrings = "0.19.0"
 mkdocstrings-python = "0.8.2"
 mknotebooks = "0.7.1"
 mike = "^1.1.2"
 
 [tool.poetry.group.test.dependencies]
-ruff = "0.0.241"
+ruff = "0.0.275"
 pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-html = "^3.1.1"
 pylic = "^3.4.0"
 
 [tool.ruff]
-ignore = ["E501"]
+select = ["E", "F", "I", "W", "B", "RUF", "NPY", "PD", "ERA", "PTH", "SIM", "RET", "RSE", "T20", "PIE"]
+ignore = ["E501", "B006", "B905", "B017", "W605", "RUF001", "RUF013", "PD901", "SIM118", "RET503"]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".eggs",
     ".git",
     ".gitignore",
     ".ruff_cache",
     ".tox",
```

### Comparing `edsteva-0.2.0/setup.py` & `edsteva-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
  'pgpasslib>=1.1.0,<2.0.0',
  'psycopg2-binary>=2.9.3,<3.0.0',
  'pyarrow>=0.15,<0.17.0',
  'pyspark>=2.4.3,<2.5.0']
 
 setup_kwargs = {
     'name': 'edsteva',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.',
-    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.2.0\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
+    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.2.1\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
     'author': 'Adam Remaki',
     'author_email': 'adam.remaki@aphp.fr',
     'maintainer': 'Adam Remaki',
     'maintainer_email': 'adam.remaki@aphp.fr',
     'url': 'https://github.com/aphp/edsteva',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 'edsteva.viz.dashboards.probe', 'edsteva.viz.plots',
 'edsteva.viz.plots.estimates_densities', 'edsteva.viz.plots.normalized_probe',
 'edsteva.viz.plots.probe'] package_data = \ {'': ['*']} install_requires = \
 ['altair>=5.0,<6.0', 'catalogue>=2.0.8,<3.0.0', 'ipython>=7.31.0,<8.0.0',
 'koalas>=1.8.2,<2.0.0', 'loguru==0.7.0', 'numpy<1.20.0', 'pandas>=1.3,<2.0',
 'pgpasslib>=1.1.0,<2.0.0', 'psycopg2-binary>=2.9.3,<3.0.0',
 'pyarrow>=0.15,<0.17.0', 'pyspark>=2.4.3,<2.5.0'] setup_kwargs = { 'name':
-'edsteva', 'version': '0.2.0', 'description': 'EDS-TeVa provides a set of tools
+'edsteva', 'version': '0.2.1', 'description': 'EDS-TeVa provides a set of tools
 that aims at modeling the adoption over time and across space of the Electronic
 Health Records.', 'long_description': '
        \nDISCLAIMER:EDS-TeVa is intended to be a module of EDS-Scikit\n
 \n\n
                                      \n\n
                                 \n [EDS-TeVa]\n
    \n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://
@@ -47,15 +47,15 @@
 tools that aims at modeling the adoption over time and across space of the
 Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders
 of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:
 \n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa
 through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning
 the library version in your projects, or use a strict package manager like
 [Poetry](https://python-poetry.org/).\n\n```\npip install
-edsteva==0.2.0\n```\n## Example\n\nA scientific paper is currently being
+edsteva==0.2.1\n```\n## Example\n\nA scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given.\n\n## Acknowledgement\n\nWe would like to thank
 [Assistance Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP
 Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
 'author': 'Adam Remaki', 'author_email': 'adam.remaki@aphp.fr', 'maintainer':
```

### Comparing `edsteva-0.2.0/PKG-INFO` & `edsteva-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsteva
-Version: 0.2.0
+Version: 0.2.1
 Summary: EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.
 Home-page: https://github.com/aphp/edsteva
 License: BSD 3-Clause
 Keywords: OMOP,Data Analysis,Electronic health record
 Author: Adam Remaki
 Author-email: adam.remaki@aphp.fr
 Maintainer: Adam Remaki
@@ -89,15 +89,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.2.0
+pip install edsteva==0.2.1
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edsteva Version: 0.2.0 Summary: EDS-TeVa provides a
+Metadata-Version: 2.1 Name: edsteva Version: 0.2.1 Summary: EDS-TeVa provides a
 set of tools that aims at modeling the adoption over time and across space of
 the Electronic Health Records. Home-page: https://github.com/aphp/edsteva
 License: BSD 3-Clause Keywords: OMOP,Data Analysis,Electronic health record
 Author: Adam Remaki Author-email: adam.remaki@aphp.fr Maintainer: Adam Remaki
 Maintainer-email: adam.remaki@aphp.fr Requires-Python: >=3.7.1,<3.8.0
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
@@ -28,14 +28,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.2.0 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.1 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

