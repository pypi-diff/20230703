# Comparing `tmp/lightwood-23.6.4.0.tar.gz` & `tmp/lightwood-23.7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwood-23.6.4.0.tar", last modified: Mon Jun 26 14:15:23 2023, max compression
+gzip compressed data, was "lightwood-23.7.1.0.tar", last modified: Mon Jul  3 13:10:54 2023, max compression
```

## Comparing `lightwood-23.6.4.0.tar` & `lightwood-23.7.1.0.tar`

### file list

```diff
@@ -1,160 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/onehot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.778922 lightwood-23.6.4.0/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.778922 lightwood-23.6.4.0/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51442 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25300 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/categorical/simple_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.246830 lightwood-23.7.1.0/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.250831 lightwood-23.7.1.0/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.254831 lightwood-23.7.1.0/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.254831 lightwood-23.7.1.0/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:10:54.242830 lightwood-23.7.1.0/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-03 13:10:54.000000 lightwood-23.7.1.0/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 13:10:53.000000 lightwood-23.7.1.0/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 13:10:54.258831 lightwood-23.7.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-03 13:10:41.000000 lightwood-23.7.1.0/setup.py
```

### Comparing `lightwood-23.6.4.0/LICENSE` & `lightwood-23.7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/PKG-INFO` & `lightwood-23.7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.6.4.0
+Version: 23.7.1.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -216,15 +216,15 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: image
 Provides-Extra: extra
-Provides-Extra: extra_ts
 Provides-Extra: dev
-Provides-Extra: quantum
+Provides-Extra: extra_ts
 Provides-Extra: xai
-Provides-Extra: image
 Provides-Extra: audio
+Provides-Extra: quantum
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.6.4.0/README.md` & `lightwood-23.7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/__init__.py` & `lightwood-23.7.1.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/analyze.py` & `lightwood-23.7.1.0/lightwood/analysis/analyze.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import Dict, List, Tuple, Optional
 
+import numpy as np
 from dataprep_ml import StatisticalAnalysis
 
 from lightwood.helpers.log import log
 from type_infer.dtype import dtype
 from lightwood.ensemble import BaseEnsemble
 from lightwood.analysis.base import BaseAnalysisBlock
 from lightwood.data.encoded_ds import EncodedDs
 from lightwood.encoder.text.pretrained import PretrainedLangEncoder
-from lightwood.api.types import ModelAnalysis, TimeseriesSettings, PredictionArguments
+from lightwood.api.types import ModelAnalysis, ProblemDefinition, PredictionArguments
 
 
 def model_analyzer(
     predictor: BaseEnsemble,
     data: EncodedDs,
     train_data: EncodedDs,
     stats_info: StatisticalAnalysis,
     target: str,
-    tss: TimeseriesSettings,
+    pdef: ProblemDefinition,
     dtype_dict: Dict[str, str],
     accuracy_functions,
     ts_analysis: Dict,
     analysis_blocks: Optional[List[BaseAnalysisBlock]] = []
 ) -> Tuple[ModelAnalysis, Dict[str, object]]:
     """
     Analyses model on a validation subset to evaluate accuracy, estimate feature importance and generate a
@@ -35,62 +36,72 @@
     calling the `.explain()` method of all analysis blocks when generating predictions.
 
     model_analysis: `ModelAnalysis` object that contains core analysis metrics, not necessarily needed when predicting.
     """
 
     runtime_analyzer = {}
     data_type = dtype_dict[target]
+    tss = pdef.timeseries_settings
 
     # retrieve encoded data representations
     encoded_train_data = train_data
     encoded_val_data = data
     data = encoded_val_data.data_frame
     input_cols = list([col for col in data.columns if col != target])
 
-    # predictive task
-    is_numerical = data_type in (dtype.integer, dtype.float, dtype.num_tsarray, dtype.quantity)
-    is_classification = data_type in (dtype.categorical, dtype.binary, dtype.cat_tsarray)
-    is_multi_ts = tss.is_timeseries and tss.horizon > 1
-    has_pretrained_text_enc = any([isinstance(enc, PretrainedLangEncoder)
-                                   for enc in encoded_train_data.encoders.values()])
-
-    # raw predictions for validation dataset
-    args = {} if not is_classification else {"predict_proba": True}
-    filtered_df = encoded_val_data.data_frame
-    normal_predictions = None
-
-    if len(analysis_blocks) > 0:
-        normal_predictions = predictor(encoded_val_data, args=PredictionArguments.from_dict(args))
-        normal_predictions = normal_predictions.set_index(encoded_val_data.data_frame.index)
-
-    # ------------------------- #
-    # Run analysis blocks, both core and user-defined
-    # ------------------------- #
-    kwargs = {
-        'predictor': predictor,
-        'target': target,
-        'input_cols': input_cols,
-        'dtype_dict': dtype_dict,
-        'normal_predictions': normal_predictions,
-        'data': filtered_df,
-        'train_data': train_data,
-        'encoded_val_data': encoded_val_data,
-        'is_classification': is_classification,
-        'is_numerical': is_numerical,
-        'is_multi_ts': is_multi_ts,
-        'stats_info': stats_info,
-        'tss': tss,
-        'ts_analysis': ts_analysis,
-        'accuracy_functions': accuracy_functions,
-        'has_pretrained_text_enc': has_pretrained_text_enc
-    }
-
-    for block in analysis_blocks:
-        log.info("The block %s is now running its analyze() method", block.__class__.__name__)
-        runtime_analyzer = block.analyze(runtime_analyzer, **kwargs)
+    if not pdef.embedding_only:
+        # predictive task
+        is_numerical = data_type in (dtype.integer, dtype.float, dtype.num_tsarray, dtype.quantity)
+        is_classification = data_type in (dtype.categorical, dtype.binary, dtype.cat_tsarray)
+        is_multi_ts = tss.is_timeseries and tss.horizon > 1
+        has_pretrained_text_enc = any([isinstance(enc, PretrainedLangEncoder)
+                                       for enc in encoded_train_data.encoders.values()])
+
+        # raw predictions for validation dataset
+        args = {} if not is_classification else {"predict_proba": True}
+        normal_predictions = None
+
+        if len(analysis_blocks) > 0:
+            if tss.is_timeseries:
+                # we retrieve the first entry per group (closest to supervision cutoff)
+                if tss.group_by:
+                    encoded_val_data.data_frame['__mdb_val_idx'] = np.arange(len(encoded_val_data))
+                    idxs = encoded_val_data.data_frame.groupby(by=tss.group_by).first()['__mdb_val_idx'].values
+                    encoded_val_data.data_frame = encoded_val_data.data_frame.iloc[idxs, :]
+                    if encoded_val_data.cache_built:
+                        encoded_val_data.X_cache = encoded_val_data.X_cache[idxs, :]
+                        encoded_val_data.Y_cache = encoded_val_data.Y_cache[idxs, :]
+            normal_predictions = predictor(encoded_val_data, args=PredictionArguments.from_dict(args))
+            normal_predictions = normal_predictions.set_index(encoded_val_data.data_frame.index)
+
+        # ------------------------- #
+        # Run analysis blocks, both core and user-defined
+        # ------------------------- #
+        kwargs = {
+            'predictor': predictor,
+            'target': target,
+            'input_cols': input_cols,
+            'dtype_dict': dtype_dict,
+            'normal_predictions': normal_predictions,
+            'data': encoded_val_data.data_frame,
+            'train_data': train_data,
+            'encoded_val_data': encoded_val_data,
+            'is_classification': is_classification,
+            'is_numerical': is_numerical,
+            'is_multi_ts': is_multi_ts,
+            'stats_info': stats_info,
+            'tss': tss,
+            'ts_analysis': ts_analysis,
+            'accuracy_functions': accuracy_functions,
+            'has_pretrained_text_enc': has_pretrained_text_enc
+        }
+
+        for block in analysis_blocks:
+            log.info("The block %s is now running its analyze() method", block.__class__.__name__)
+            runtime_analyzer = block.analyze(runtime_analyzer, **kwargs)
 
     # ------------------------- #
     # Populate ModelAnalysis object
     # ------------------------- #
     model_analysis = ModelAnalysis(
         accuracies=runtime_analyzer.get('score_dict', {}),
         accuracy_histogram=runtime_analyzer.get('acc_histogram', {}),
```

### Comparing `lightwood-23.6.4.0/lightwood/analysis/base.py` & `lightwood-23.7.1.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/explain.py` & `lightwood-23.7.1.0/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.7.1.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.7.1.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.7.1.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/helpers/pyod.py` & `lightwood-23.7.1.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/helpers/shap.py` & `lightwood-23.7.1.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/base.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/calibrate.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/icp.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/metrics.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/nc.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/norm.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nc/util.py` & `lightwood-23.7.1.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.7.1.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/api/__init__.py` & `lightwood-23.7.1.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/api/high_level.py` & `lightwood-23.7.1.0/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/api/json_ai.py` & `lightwood-23.7.1.0/lightwood/api/json_ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # TODO: _add_implicit_values unit test ensures NO changes for a fully specified file.
+import inspect
 from copy import deepcopy
+
+from type_infer.dtype import dtype
 from type_infer.base import TypeInformation
 from dataprep_ml import StatisticalAnalysis
 
+from lightwood.helpers.log import log
 from lightwood.helpers.templating import call, inline_dict, align
-from lightwood.helpers.templating import _consolidate_analysis_blocks
-from type_infer.dtype import dtype
+from lightwood.helpers.templating import _consolidate_analysis_blocks, _add_cls_kwarg
 from lightwood.api.types import (
     JsonAI,
     ProblemDefinition,
 )
-import inspect
-from lightwood.helpers.log import log
 from lightwood.__about__ import __version__ as lightwood_version
-
+import lightwood.ensemble
 
 # For custom modules, we create a module loader with necessary imports below
 IMPORT_EXTERNAL_DIRS = """
 for import_dir in [os.path.join(os.path.expanduser('~/lightwood_modules'), lightwood_version.replace('.', '_')), os.path.join('/etc/lightwood_modules', lightwood_version.replace('.', '_'))]:
     if os.path.exists(import_dir) and os.access(import_dir, os.R_OK):
         for file_name in list(os.walk(import_dir))[0][2]:
             if file_name[-3:] != '.py':
@@ -531,37 +532,37 @@
     :params: json_ai: ``JsonAI`` object that describes the ML pipeline that may not have every detail fully specified.
 
     :returns: ``JSONAI`` object with all necessary parameters that were previously left unmentioned filled in.
     """
     problem_definition = json_ai.problem_definition
     tss = problem_definition.timeseries_settings
     is_ts = tss.is_timeseries
+    # tsa_val = "self.ts_analysis" if is_ts else None  # TODO: remove
+    mixers = json_ai.model['args']['submodels']
 
     # Add implicit ensemble arguments
-    json_ai.model["args"]["target"] = json_ai.model["args"].get("target", "$target")
-    json_ai.model["args"]["data"] = json_ai.model["args"].get("data", "encoded_test_data")
-    json_ai.model["args"]["mixers"] = json_ai.model["args"].get("mixers", "$mixers")
-    json_ai.model["args"]["fit"] = json_ai.model["args"].get("fit", True)
-    json_ai.model["args"]["args"] = json_ai.model["args"].get("args", "$pred_args")  # TODO correct?
-
-    # @TODO: change this to per-parameter basis and signature inspection
-    if json_ai.model["module"] in ("BestOf", "ModeEnsemble", "WeightedMeanEnsemble"):
-        json_ai.model["args"]["accuracy_functions"] = json_ai.model["args"].get("accuracy_functions",
-                                                                                "$accuracy_functions")
-
-    if json_ai.model["module"] in ("BestOf", "TsStackedEnsemble", "WeightedMeanEnsemble"):
-        tsa_val = "self.ts_analysis" if is_ts else None
-        json_ai.model["args"]["ts_analysis"] = json_ai.model["args"].get("ts_analysis", tsa_val)
-
-    if json_ai.model["module"] in ("MeanEnsemble", "ModeEnsemble", "StackedEnsemble", "TsStackedEnsemble",
-                                   "WeightedMeanEnsemble"):
-        json_ai.model["args"]["dtype_dict"] = json_ai.model["args"].get("dtype_dict", "$dtype_dict")
+    param_pairs = {
+        'target': json_ai.model["args"].get("target", "$target"),
+        'data': json_ai.model["args"].get("data", "encoded_test_data"),
+        'mixers': json_ai.model["args"].get("mixers", "$mixers"),
+        'fit': json_ai.model["args"].get("fit", True),
+        'args': json_ai.model["args"].get("args", "$pred_args"),
+        'accuracy_functions': json_ai.model["args"].get("accuracy_functions", "$accuracy_functions"),
+        'ts_analysis': json_ai.model["args"].get("ts_analysis", "self.ts_analysis" if is_ts else None),
+        'dtype_dict': json_ai.model["args"].get("dtype_dict", "$dtype_dict"),
+    }
+    ensemble_cls = getattr(lightwood.ensemble, json_ai.model["module"])
+    filtered_params = {}
+    for p_name, p_value in param_pairs.items():
+        _add_cls_kwarg(ensemble_cls, filtered_params, p_name, p_value)
+
+    json_ai.model["args"] = filtered_params
+    json_ai.model["args"]['submodels'] = mixers  # add mixers back in
 
     # Add implicit mixer arguments
-    mixers = json_ai.model['args']['submodels']
     for i in range(len(mixers)):
         if not mixers[i].get("args", False):
             mixers[i]["args"] = {}
 
         if mixers[i]["module"] == "Unit":
             continue
 
@@ -681,15 +682,15 @@
                 "pct_test": 0.1,
             },
         },
         "analyzer": {
             "module": "model_analyzer",
             "args": {
                 "stats_info": "$statistical_analysis",
-                "tss": "$problem_definition.timeseries_settings",
+                "pdef": "$problem_definition",
                 "accuracy_functions": "$accuracy_functions",
                 "predictor": "$ensemble",
                 "data": "encoded_test_data",
                 "train_data": "encoded_train_data",
                 "target": "$target",
                 "dtype_dict": "$dtype_dict",
                 "analysis_blocks": "$analysis_blocks",
@@ -1166,15 +1167,20 @@
 
 # Create feature vectors from data
 log.info(f'[Learn phase 5/{n_phases}] - Feature generation')
 enc_train_test = self.featurize(train_dev_test)
 
 # Prepare mixers
 log.info(f'[Learn phase 6/{n_phases}] - Mixer training')
-self.fit(enc_train_test)
+if not self.problem_definition.embedding_only:
+    self.fit(enc_train_test)
+else:
+    self.mixers = []
+    self.ensemble = Embedder(self.target, mixers=list(), data=enc_train_test['train'])
+    self.supports_proba = self.ensemble.supports_proba
 
 # Analyze the ensemble
 log.info(f'[Learn phase 7/{n_phases}] - Ensemble analysis')
 self.analyze_ensemble(enc_train_test)
 
 # ------------------------ #
 # Enable model partial fit AFTER it is trained and evaluated for performance with the appropriate train/dev/test splits.
@@ -1217,17 +1223,25 @@
 
 # Featurize the data
 log.info(f'[Predict phase 2/{{n_phases}}] - Feature generation')
 encoded_ds = self.featurize({{"predict_data": data}})["predict_data"]
 encoded_data = encoded_ds.get_encoded_data(include_target=False)
 
 log.info(f'[Predict phase 3/{{n_phases}}] - Calling ensemble')
-df = self.ensemble(encoded_ds, args=self.pred_args)
+if self.pred_args.return_embedding:
+    embedder = Embedder(self.target, mixers=list(), data=encoded_ds)
+    df = embedder(encoded_ds, args=self.pred_args)
+else:
+    df = self.ensemble(encoded_ds, args=self.pred_args)
 
-if not self.pred_args.all_mixers:
+if not(any(
+            [self.pred_args.all_mixers,
+             self.pred_args.return_embedding,
+             self.problem_definition.embedding_only]
+        )):
     log.info(f'[Predict phase 4/{{n_phases}}] - Analyzing output')
     df, global_insights = {call(json_ai.explainer)}
     self.global_insights = {{**self.global_insights, **global_insights}}
 
 self.feature_cache = dict()  # empty feature cache to avoid large predictor objects
 
 return df
```

### Comparing `lightwood-23.6.4.0/lightwood/api/predictor.py` & `lightwood-23.7.1.0/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/api/types.py` & `lightwood-23.7.1.0/lightwood/api/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
     expected_additional_time: Optional[int]
     time_aim: Optional[float]
     target_weights: Optional[List[float]]
     positive_domain: bool
     timeseries_settings: TimeseriesSettings
     anomaly_detection: bool
     use_default_analysis: bool
+    embedding_only: bool
     dtype_dict: Optional[dict]
     ignore_features: List[str]
     fit_on_all: bool
     strict_mode: bool
     seed_nr: int
 
     @staticmethod
@@ -216,14 +217,15 @@
         positive_domain = obj.get('positive_domain', False)
         dtype_dict = obj.get('dtype_dict', {})
         timeseries_settings = TimeseriesSettings.from_dict(obj.get('timeseries_settings', {}))
         anomaly_detection = obj.get('anomaly_detection', False)
         ignore_features = obj.get('ignore_features', [])
         fit_on_all = obj.get('fit_on_all', True)
         use_default_analysis = obj.get('use_default_analysis', True)
+        embedding_only = obj.get('embedding_only', False)
         strict_mode = obj.get('strict_mode', True)
         seed_nr = obj.get('seed_nr', 1)
         problem_definition = ProblemDefinition(
             target=target,
             pct_invalid=pct_invalid,
             unbias_target=unbias_target,
             seconds_per_mixer=seconds_per_mixer,
@@ -233,14 +235,15 @@
             target_weights=target_weights,
             positive_domain=positive_domain,
             timeseries_settings=timeseries_settings,
             anomaly_detection=anomaly_detection,
             dtype_dict=dtype_dict,
             ignore_features=ignore_features,
             use_default_analysis=use_default_analysis,
+            embedding_only=embedding_only,
             fit_on_all=fit_on_all,
             strict_mode=strict_mode,
             seed_nr=seed_nr
         )
 
         return problem_definition
 
@@ -449,14 +452,15 @@
     mixer_weights: list = None
     fixed_confidence: Union[int, float, None] = None
     anomaly_cooldown: int = 1
     forecast_offset: int = 0
     simple_ts_bounds: bool = False
     time_format: str = ''
     force_ts_infer: bool = False
+    return_embedding: bool = False
 
     @staticmethod
     def from_dict(obj: Dict):
         """
         Creates a ``PredictionArguments`` object from a python dictionary with necessary specifications.
 
         :param obj: A python dictionary with the necessary features for the ``PredictionArguments`` class.
@@ -470,25 +474,27 @@
         mixer_weights = obj.get('mixer_weights', PredictionArguments.mixer_weights)
         fixed_confidence = obj.get('fixed_confidence', PredictionArguments.fixed_confidence)
         anomaly_cooldown = obj.get('anomaly_cooldown', PredictionArguments.anomaly_cooldown)
         forecast_offset = obj.get('forecast_offset', PredictionArguments.forecast_offset)
         simple_ts_bounds = obj.get('simple_ts_bounds', PredictionArguments.simple_ts_bounds)
         time_format = obj.get('time_format', PredictionArguments.time_format)
         force_ts_infer = obj.get('force_ts_infer', PredictionArguments.force_ts_infer)
+        return_embedding = obj.get('return_embedding', PredictionArguments.return_embedding)
 
         pred_args = PredictionArguments(
             predict_proba=predict_proba,
             all_mixers=all_mixers,
             mixer_weights=mixer_weights,
             fixed_confidence=fixed_confidence,
             anomaly_cooldown=anomaly_cooldown,
             forecast_offset=forecast_offset,
             simple_ts_bounds=simple_ts_bounds,
             time_format=time_format,
             force_ts_infer=force_ts_infer,
+            return_embedding=return_embedding,
         )
 
         return pred_args
 
     def to_dict(self, encode_json=False) -> Dict[str, Json]:
         """
         Creates a python dictionary from the ``PredictionArguments`` object
```

### Comparing `lightwood-23.6.4.0/lightwood/data/encoded_ds.py` & `lightwood-23.7.1.0/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/data/timeseries_analyzer.py` & `lightwood-23.7.1.0/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/data/timeseries_transform.py` & `lightwood-23.7.1.0/lightwood/data/timeseries_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         original_df['original_index'] = None
 
     secondary_type_dict = {}
     if dtype_dict[oby] in (dtype.date, dtype.integer, dtype.float):
         secondary_type_dict[oby] = dtype_dict[oby]
 
     original_df[f'__mdb_original_{oby}'] = original_df[oby]
+    original_df = _ts_to_obj(original_df, [oby] + tss.historical_columns)
     group_lengths = []
     if len(gb_arr) > 0:
         df_arr = []
         for _, df in original_df.groupby(gb_arr):
             df_arr.append(df.sort_values(by=oby))
             group_lengths.append(len(df))
     else:
@@ -132,38 +133,38 @@
                 df_arr[i] = df_arr[i].loc[new_index]
             else:
                 if pred_args.force_ts_infer:
                     df_arr[i] = _ts_infer_next_row(subdf, oby)  # force-infer out-of-sample forecast in default mode
                 make_preds = [True for _ in range(len(df_arr[i]))]
             df_arr[i]['__make_predictions'] = make_preds
 
-    if len(original_df) > 500:
+    if len(df_arr) > 1 and len(original_df) > 5000:
         # @TODO: restore possibility to override this with args
-        nr_procs = get_nr_procs(original_df)
+        biggest_sub_df = df_arr[np.argmax(group_lengths)]
+        nr_procs = min(get_nr_procs(biggest_sub_df), len(df_arr))
         log.info(f'Using {nr_procs} processes to reshape.')
-        pool = mp.Pool(processes=nr_procs)
-        # Make type `object` so that dataframe cells can be python lists
-        df_arr = pool.map(partial(_ts_to_obj, historical_columns=[oby] + tss.historical_columns), df_arr)
-        df_arr = pool.map(
-            partial(
-                _ts_add_previous_rows, order_cols=[oby] + tss.historical_columns, window=window),
-            df_arr)
-        df_arr = pool.map(partial(_ts_add_future_target, target=target, horizon=tss.horizon,
-                                  data_dtype=tss.target_type, mode=mode),
-                          df_arr)
+        with mp.Pool(processes=nr_procs) as pool:
+            df_arr = pool.map(
+                partial(_ts_add_previous_rows, order_cols=[oby] + tss.historical_columns, window=window),
+                df_arr
+            )
 
-        if tss.use_previous_target:
             df_arr = pool.map(
-                partial(_ts_add_previous_target, target=target, window=tss.window),
-                df_arr)
-        pool.close()
-        pool.join()
+                partial(_ts_add_future_target, target=target, horizon=tss.horizon,
+                        data_dtype=tss.target_type, mode=mode),
+                df_arr
+            )
+
+            if tss.use_previous_target:
+                df_arr = pool.map(
+                    partial(_ts_add_previous_target, target=target, window=tss.window),
+                    df_arr
+                )
     else:
         for i in range(n_groups):
-            df_arr[i] = _ts_to_obj(df_arr[i], historical_columns=[oby] + tss.historical_columns)
             df_arr[i] = _ts_add_previous_rows(df_arr[i],
                                               order_cols=[oby] + tss.historical_columns, window=window)
             df_arr[i] = _ts_add_future_target(df_arr[i], target=target, horizon=tss.horizon,
                                               data_dtype=tss.target_type, mode=mode)
             if tss.use_previous_target:
                 df_arr[i] = _ts_add_previous_target(df_arr[i], target=target, window=tss.window)
```

### Comparing `lightwood-23.6.4.0/lightwood/encoder/__init__.py` & `lightwood-23.7.1.0/lightwood/encoder/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from lightwood.encoder.image.img_2_vec import Img2VecEncoder
 from lightwood.encoder.numeric.numeric import NumericEncoder
 from lightwood.encoder.numeric.ts_numeric import TsNumericEncoder
 from lightwood.encoder.array.ts_num_array import TsArrayNumericEncoder
 from lightwood.encoder.text.short import ShortTextEncoder
 from lightwood.encoder.text.vocab import VocabularyEncoder
 from lightwood.encoder.text.rnn import RnnEncoder as TextRnnEncoder
+from lightwood.encoder.categorical.simple_label import SimpleLabelEncoder
 from lightwood.encoder.categorical.onehot import OneHotEncoder
 from lightwood.encoder.categorical.binary import BinaryEncoder
 from lightwood.encoder.categorical.autoencoder import CategoricalAutoEncoder
 from lightwood.encoder.time_series.ts import TimeSeriesEncoder
 from lightwood.encoder.array.array import ArrayEncoder, NumArrayEncoder, CatArrayEncoder
 from lightwood.encoder.categorical.multihot import MultiHotEncoder
 from lightwood.encoder.array.ts_cat_array import TsCatArrayEncoder
 from lightwood.encoder.text.pretrained import PretrainedLangEncoder
 from lightwood.encoder.audio import MFCCEncoder
 
 
 __all__ = ['BaseEncoder', 'DatetimeEncoder', 'Img2VecEncoder', 'NumericEncoder', 'TsNumericEncoder',
            'TsArrayNumericEncoder', 'ShortTextEncoder', 'VocabularyEncoder', 'TextRnnEncoder', 'OneHotEncoder',
            'CategoricalAutoEncoder', 'TimeSeriesEncoder', 'ArrayEncoder', 'MultiHotEncoder', 'TsCatArrayEncoder',
-           'NumArrayEncoder', 'CatArrayEncoder',
+           'NumArrayEncoder', 'CatArrayEncoder', 'SimpleLabelEncoder',
            'PretrainedLangEncoder', 'BinaryEncoder', 'DatetimeNormalizerEncoder', 'MFCCEncoder']
```

### Comparing `lightwood-23.6.4.0/lightwood/encoder/array/array.py` & `lightwood-23.7.1.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.7.1.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.7.1.0/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/audio/mfcc.py` & `lightwood-23.7.1.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/base.py` & `lightwood-23.7.1.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/categorical/binary.py` & `lightwood-23.7.1.0/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/categorical/gym.py` & `lightwood-23.7.1.0/lightwood/encoder/categorical/gym.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import time
 import torch
 
 import numpy as np
 from lightwood.helpers.torch import LightwoodAutocast
+from lightwood.helpers.log import log
 
 
 class Gym:
 
     def __init__(self, model, optimizer, scheduler, loss_criterion, device,
                  name=None, input_encoder=None, output_encoder=None):
         """
@@ -42,14 +43,16 @@
             for i, data in enumerate(train_data_loader, 0):
                 if custom_train_func is None:
                     input, real = data
 
                     with LightwoodAutocast():
                         if self.input_encoder is not None:
                             input = self.input_encoder(input)
+                            if len(input.shape) < 2:
+                                input = input.unsqueeze(-1)
                         if self.output_encoder is not None:
                             real = self.output_encoder(real)
 
                         input = input.to(self.device)
                         real = real.to(self.device)
 
                         predicted = self.model(input)
@@ -63,14 +66,16 @@
                     self.optimizer.zero_grad()
                 else:
                     loss = custom_train_func(self.model, data, self)
 
                 running_loss += loss.item()
                 error = running_loss / (i + 1)
 
+            # end of epoch checks
+            log.debug(f'Categorical AutoEncoder train loss at epoch {epoch}: {round(error, 9)}')
             if epoch % eval_every_x_epochs == 0:
                 if test_data_loader is not None:
                     test_running_loss = 0.0
                     test_error = 0
                     self.model = self.model.eval()
                     real_buff = []
                     predicted_buff = []
@@ -94,14 +99,15 @@
                             predicted_buff.append(predicted.tolist())
 
                             loss = self.loss_criterion(predicted, real)
                         else:
                             with torch.no_grad():
                                 loss = custom_test_func(self.model, data, self)
 
+                        log.debug(f'Categorical AutoEncoder val loss at epoch {epoch}: {round(loss, 9)}')
                         test_running_loss += loss.item()
                         test_error = test_running_loss / (i + 1)
                 else:
                     test_error = error
                     real_buff = None
                     predicted_buff = None
```

### Comparing `lightwood-23.6.4.0/lightwood/encoder/categorical/multihot.py` & `lightwood-23.7.1.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/categorical/onehot.py` & `lightwood-23.7.1.0/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/datetime/datetime.py` & `lightwood-23.7.1.0/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-23.7.1.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/helpers.py` & `lightwood-23.7.1.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/identity/identity.py` & `lightwood-23.7.1.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.7.1.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.7.1.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/numeric/numeric.py` & `lightwood-23.7.1.0/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-23.7.1.0/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.7.1.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.7.1.0/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/pretrained.py` & `lightwood-23.7.1.0/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/rnn.py` & `lightwood-23.7.1.0/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/short.py` & `lightwood-23.7.1.0/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/tfidf.py` & `lightwood-23.7.1.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/text/vocab.py` & `lightwood-23.7.1.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.7.1.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/time_series/rnn.py` & `lightwood-23.7.1.0/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/encoder/time_series/ts.py` & `lightwood-23.7.1.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/__init__.py` & `lightwood-23.7.1.0/lightwood/ensemble/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from lightwood.ensemble.base import BaseEnsemble
+from lightwood.ensemble.identity import IdentityEnsemble
+from lightwood.ensemble.embed import Embedder
 from lightwood.ensemble.best_of import BestOf
 from lightwood.ensemble.mean_ensemble import MeanEnsemble
 from lightwood.ensemble.mode_ensemble import ModeEnsemble
 from lightwood.ensemble.stacked_ensemble import StackedEnsemble
 from lightwood.ensemble.ts_stacked_ensemble import TsStackedEnsemble
 from lightwood.ensemble.weighted_mean_ensemble import WeightedMeanEnsemble
 
 __all__ = ['BaseEnsemble', 'BestOf', 'MeanEnsemble', 'ModeEnsemble', 'WeightedMeanEnsemble', 'StackedEnsemble',
-           'TsStackedEnsemble']
+           'TsStackedEnsemble', 'Embedder', 'IdentityEnsemble']
```

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/base.py` & `lightwood-23.7.1.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/best_of.py` & `lightwood-23.7.1.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.7.1.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.7.1.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.7.1.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.7.1.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.7.1.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/__init__.py` & `lightwood-23.7.1.0/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/device.py` & `lightwood-23.7.1.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/general.py` & `lightwood-23.7.1.0/lightwood/helpers/general.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/io.py` & `lightwood-23.7.1.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/log.py` & `lightwood-23.7.1.0/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/parallelism.py` & `lightwood-23.7.1.0/lightwood/helpers/parallelism.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
         except ValueError:
             n = 1
         return n
     elif os.name == 'nt':
         return 1
     else:
         available_mem = psutil.virtual_memory().available
-        max_per_proc_usage = 0.2 * pow(10, 9)
+        max_per_proc_usage = 2 * pow(10, 8)
 
         if df is not None:
             max_per_proc_usage += df.memory_usage(index=True, deep=True).sum()
-        proc_count = int(min(mp.cpu_count(), available_mem // max_per_proc_usage)) - 1
+        proc_count = min(mp.cpu_count(), available_mem // max_per_proc_usage) - 1
 
         return max(proc_count, 1)
 
 
 def run_mut_method(obj: object, arg: object, method: str, identifier: str) -> str:
     try:
         obj.__getattribute__(method)(arg)
```

### Comparing `lightwood-23.6.4.0/lightwood/helpers/templating.py` & `lightwood-23.7.1.0/lightwood/helpers/templating.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from typing import Callable
 from collections import deque
 
+import inspect
 import numpy as np
 
 from type_infer.dtype import dtype
 
 
 def is_allowed(v):
     if '(' in str(v):
@@ -127,7 +129,17 @@
         raise Exception("Cycle detected in analysis blocks dependencies, please review and try again!")
 
     sorted_blocks = []
     for idx in sorted_dag:
         sorted_blocks.append(block_objs[idx2block[idx]])
 
     return sorted_blocks
+
+
+def _add_cls_kwarg(cls: Callable, kwargs: dict, key: str, value):
+    """
+    Adds arguments to the `kwargs` dictionary if the key-value pair is valid for the `cls` class signature.
+    """
+    if key in [p.name for p in inspect.signature(cls).parameters.values()]:
+        kwargs[key] = value
+
+    return kwargs
```

### Comparing `lightwood-23.6.4.0/lightwood/helpers/text.py` & `lightwood-23.7.1.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/torch.py` & `lightwood-23.7.1.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/helpers/ts.py` & `lightwood-23.7.1.0/lightwood/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/__init__.py` & `lightwood-23.7.1.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/arima.py` & `lightwood-23.7.1.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/base.py` & `lightwood-23.7.1.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/ets.py` & `lightwood-23.7.1.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/gluonts.py` & `lightwood-23.7.1.0/lightwood/mixer/gluonts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/default_net.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/ranger.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/helpers/ts.py` & `lightwood-23.7.1.0/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/lightgbm.py` & `lightwood-23.7.1.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/lightgbm_array.py` & `lightwood-23.7.1.0/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/neural.py` & `lightwood-23.7.1.0/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/neural_ts.py` & `lightwood-23.7.1.0/lightwood/mixer/neural_ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/nhits.py` & `lightwood-23.7.1.0/lightwood/mixer/nhits.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.supports_proba = False
         self.target = target
         self.window = window
         self.horizon = horizon
         self.dtype_dict = dtype_dict
         self.ts_analysis = ts_analysis
         self.grouped_by = ['__default'] if not ts_analysis['tss'].group_by else ts_analysis['tss'].group_by
+        self.group_boundaries = {}  # stores last observed timestamp per series
         self.train_args = train_args.get('trainer_args', {}) if train_args else {}
         self.train_args['early_stop_patience_steps'] = self.train_args.get('early_stop_patience_steps', 10)
         self.conf_level = self.train_args.pop('conf_level', [90])
         for level in self.conf_level:
             assert 0 <= level <= 100, f'A provided level is not in the [0, 100] range (found: {level})'
             assert isinstance(level, int), f'A provided level is not an integer (found: {level})'
 
@@ -89,15 +90,16 @@
         log.info('Started fitting N-HITS forecasting model')
 
         # prepare data
         cat_ds = ConcatedEncodedDs([train_data, dev_data])
         oby_col = self.ts_analysis["tss"].order_by
         gby = self.ts_analysis["tss"].group_by if self.ts_analysis["tss"].group_by else []
         df = deepcopy(cat_ds.data_frame)
-        Y_df = self._make_initial_df(df)
+        Y_df = self._make_initial_df(df, mode='train')
+        self.group_boundaries = self._set_boundary(Y_df, gby)
         if gby:
             n_time = df[gby].value_counts().min()
         else:
             n_time = len(df[f'__mdb_original_{oby_col}'].unique())
         n_ts_val = max(int(.1 * n_time), self.horizon)  # at least self.horizon to validate on
 
         # train the model
@@ -126,17 +128,16 @@
                 log.info(f'Window {self.window} is too long for data provided (group: {df[gby].value_counts()[::-1].index[0]}), reducing window to {new_window}.')  # noqa
             model = NHITS(h=n_time_out, input_size=self.window, **self.train_args, loss=MQLoss(level=self.conf_level))
             self.model = NeuralForecast(models=[model], freq=self.ts_analysis['sample_freqs']['__default'])
             self.model.fit(df=Y_df, val_size=n_ts_val)
             log.info('Successfully trained N-HITS forecasting model.')
 
     def partial_fit(self, train_data: EncodedDs, dev_data: EncodedDs, args: Optional[dict] = None) -> None:
-        # TODO: reimplement this with automatic novel-row differential
         self.hyperparam_search = False
-        self.fit(dev_data, train_data)  # TODO: add support for passing args (e.g. n_epochs)
+        self.fit(train_data, dev_data)  # TODO: add support for passing args (e.g. n_epochs)
         self.prepared = True
 
     def __call__(self, ds: Union[EncodedDs, ConcatedEncodedDs],
                  args: PredictionArguments = PredictionArguments()) -> pd.DataFrame:
         """
         Calls the mixer to emit forecasts.
         
@@ -179,23 +180,57 @@
                 group_preds = fcst[fcst['unique_id'] == group][pred_col].tolist()[:self.horizon]
                 idx = ydf[ydf['index'] == gidx].index[0]
                 ydf.at[idx, target_col] = group_preds
 
         ydf['confidence'] = level / 100
         return ydf
 
-    def _make_initial_df(self, df):
+    def _make_initial_df(self, df, mode='inference'):
+        """
+        Prepares a dataframe for the NHITS model according to what neuralforecast expects.
+
+        If a per-group boundary exists, this method additionally drops out all observations prior to the cutoff.
+        """  # noqa
+
         oby_col = self.ts_analysis["tss"].order_by
         df = df.sort_values(by=f'__mdb_original_{oby_col}')
         df[f'__mdb_parsed_{oby_col}'] = df.index
         df = df.reset_index(drop=True)
 
         Y_df = pd.DataFrame()
         Y_df['y'] = df[self.target]
         Y_df['ds'] = df[f'__mdb_parsed_{oby_col}']
 
         if self.grouped_by != ['__default']:
             Y_df['unique_id'] = df[self.grouped_by].apply(lambda x: ','.join([elt for elt in x]), axis=1)
         else:
             Y_df['unique_id'] = '__default'
 
-        return Y_df.reset_index()
+        Y_df = Y_df.reset_index()
+
+        # filter if boundary exists
+        if mode == 'train' and self.group_boundaries:
+            filtered = []
+            grouped = Y_df.groupby(by='unique_id')
+            for group, sdf in grouped:
+                if group in self.group_boundaries:
+                    sdf = sdf[sdf['ds'].gt(self.group_boundaries[group])]
+                    if sdf.shape[0] > 0:
+                        filtered.append(sdf)
+            if filtered:
+                Y_df = pd.concat(filtered)
+
+        return Y_df
+
+    @staticmethod
+    def _set_boundary(df: pd.DataFrame, gby: list) -> Dict[str, object]:
+        """
+        Finds last observation for every series in a pre-sorted `df` given a `gby` list of columns to group by.
+        """
+        if not gby:
+            group_boundaries = {'__default': df.iloc[-1]['ds']}
+        else:
+            # could use groupby().transform('max'), but we leverage pre-sorting instead
+            grouped_df = df.groupby(by='unique_id', as_index=False).last()
+            group_boundaries = grouped_df[['unique_id', 'ds']].set_index('unique_id').to_dict()['ds']
+
+        return group_boundaries
```

### Comparing `lightwood-23.6.4.0/lightwood/mixer/prophet.py` & `lightwood-23.7.1.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/qclassic.py` & `lightwood-23.7.1.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/random_forest.py` & `lightwood-23.7.1.0/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/regression.py` & `lightwood-23.7.1.0/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/sktime.py` & `lightwood-23.7.1.0/lightwood/mixer/sktime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import inspect
 import importlib
 from copy import deepcopy
 from datetime import datetime
 from typing import Dict, Union, Optional
 
 import optuna
 import numpy as np
 import pandas as pd
 from sktime.forecasting.compose import TransformedTargetForecaster
 from sktime.forecasting.base import ForecastingHorizon, BaseForecaster
 from sktime.performance_metrics.forecasting import MeanAbsolutePercentageError
 from sktime.forecasting.statsforecast import StatsForecastAutoARIMA as AutoARIMA
 
 from lightwood.helpers.log import log
+from lightwood.helpers.templating import _add_cls_kwarg
 from lightwood.mixer.base import BaseMixer
 from lightwood.api.types import PredictionArguments
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 
 
 class SkTime(BaseMixer):
     forecaster: str
@@ -160,15 +160,15 @@
             options['suppress_warnings'] = True  # ignore warnings if possible
             options['error_action'] = 'raise'    # avoids fit() failing silently
 
             if self.model_path == 'fbprophet.Prophet':
                 options['freq'] = self.freq
 
             for k, v in options.items():
-                kwargs = self._add_forecaster_kwarg(model_class, kwargs, k, v)
+                kwargs = _add_cls_kwarg(model_class, kwargs, k, v)
 
             model_pipeline = []
 
             if self.use_stl and self.ts_analysis['stl_transforms'].get(group, False):
                 model_pipeline.insert(0, ("detrender",
                                           self.ts_analysis['stl_transforms'][group]["transformer"].detrender))
                 model_pipeline.insert(0, ("deseasonalizer",
@@ -333,23 +333,14 @@
         except Exception as e:
             log.debug(e)
             error = np.inf
 
         log.info(f'Trial got error: {error}')
         return error
 
-    def _add_forecaster_kwarg(self, forecaster: BaseForecaster, kwargs: dict, key: str, value):
-        """
-        Adds arguments to the `kwargs` dictionary if the key-value pair is valid for the `forecaster` class signature.
-        """
-        if key in [p.name for p in inspect.signature(forecaster).parameters.values()]:
-            kwargs[key] = value
-
-        return kwargs
-
     def _transform_index_to_datetime(self, series, series_oby, freq):
         series_oby = np.array([np.array(lst) for lst in series_oby])
         start = datetime.utcfromtimestamp(np.min(series_oby[series_oby != np.min(series_oby)]))
         series.index = pd.date_range(start=start, freq=freq, normalize=False, periods=series.shape[0])
         return series
 
     def _get_freq(self, delta):
```

### Comparing `lightwood-23.6.4.0/lightwood/mixer/tabtransformer.py` & `lightwood-23.7.1.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/unit.py` & `lightwood-23.7.1.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood/mixer/xgboost.py` & `lightwood-23.7.1.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/lightwood.egg-info/PKG-INFO` & `lightwood-23.7.1.0/lightwood.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.6.4.0
+Version: 23.7.1.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -216,15 +216,15 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: image
 Provides-Extra: extra
-Provides-Extra: extra_ts
 Provides-Extra: dev
-Provides-Extra: quantum
+Provides-Extra: extra_ts
 Provides-Extra: xai
-Provides-Extra: image
 Provides-Extra: audio
+Provides-Extra: quantum
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.6.4.0/lightwood.egg-info/SOURCES.txt` & `lightwood-23.7.1.0/lightwood.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 lightwood/encoder/audio/mfcc.py
 lightwood/encoder/categorical/__init__.py
 lightwood/encoder/categorical/autoencoder.py
 lightwood/encoder/categorical/binary.py
 lightwood/encoder/categorical/gym.py
 lightwood/encoder/categorical/multihot.py
 lightwood/encoder/categorical/onehot.py
+lightwood/encoder/categorical/simple_label.py
 lightwood/encoder/datetime/__init__.py
 lightwood/encoder/datetime/datetime.py
 lightwood/encoder/datetime/datetime_sin_normalizer.py
 lightwood/encoder/identity/__init__.py
 lightwood/encoder/identity/identity.py
 lightwood/encoder/image/__init__.py
 lightwood/encoder/image/img_2_vec.py
@@ -82,14 +83,16 @@
 lightwood/encoder/time_series/helpers/__init__.py
 lightwood/encoder/time_series/helpers/common.py
 lightwood/encoder/time_series/helpers/rnn_helpers.py
 lightwood/encoder/time_series/helpers/transformer_helpers.py
 lightwood/ensemble/__init__.py
 lightwood/ensemble/base.py
 lightwood/ensemble/best_of.py
+lightwood/ensemble/embed.py
+lightwood/ensemble/identity.py
 lightwood/ensemble/mean_ensemble.py
 lightwood/ensemble/mode_ensemble.py
 lightwood/ensemble/stacked_ensemble.py
 lightwood/ensemble/ts_stacked_ensemble.py
 lightwood/ensemble/weighted_mean_ensemble.py
 lightwood/helpers/__init__.py
 lightwood/helpers/constants.py
```

### Comparing `lightwood-23.6.4.0/lightwood.egg-info/requires.txt` & `lightwood-23.7.1.0/lightwood.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -31,27 +31,27 @@
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
 torchvision
-suod
-lightgbm<=3.3.3,>=3.3.0
-neuralforecast==1.5.0
 prophet==1.1
-qiskit==0.31.0
-librosa==0.8.1
-mxnet<2.0.0,>=1.6.0
 pystan==2.19.1.1
 autopep8>=1.5.7
+pillow>8.3.1
+suod
+lightgbm<=3.3.3,>=3.3.0
+mxnet<2.0.0,>=1.6.0
 pyod==1.0.4
-shap>=0.40.0
+qiskit==0.31.0
 gluonts<0.12.0,>=0.11.0
-pillow>8.3.1
+neuralforecast==1.5.0
+librosa==0.8.1
+shap>=0.40.0
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
```

### Comparing `lightwood-23.6.4.0/requirements.txt` & `lightwood-23.7.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.4.0/setup.py` & `lightwood-23.7.1.0/setup.py`

 * *Files identical despite different names*

