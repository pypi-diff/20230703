# Comparing `tmp/kappadata-1.2.9.tar.gz` & `tmp/kappadata-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappadata-1.2.9.tar", last modified: Wed Apr 12 21:53:00 2023, max compression
+gzip compressed data, was "kappadata-1.3.0.tar", last modified: Mon Jul  3 08:01:28 2023, max compression
```

## Comparing `kappadata-1.2.9.tar` & `kappadata-1.3.0.tar`

### file list

```diff
@@ -1,162 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 21:50:51.000000 kappadata-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-12 21:53:00.370054 kappadata-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-04-12 21:50:51.000000 kappadata-1.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata/
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-12 21:52:46.000000 kappadata-1.2.9/kappadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata/caching/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/caching/cached_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/caching/shared_dict_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata/collators/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/collators/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/kd_collator_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/kd_compose_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/base/kd_single_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/kd_mix_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/collators/pad_sequences_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/common/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/common/collators/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/collators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/collators/mae_finetune_mix_collator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.350054 kappadata-1.2.9/kappadata/common/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/datasets/kd_image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.354054 kappadata-1.2.9/kappadata/common/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/byol_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/imagenet_minaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/imagenet_noaug_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/mae_finetune_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.354054 kappadata-1.2.9/kappadata/common/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/kd_cifar100_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/kd_cifar10_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/transforms/norm/kd_image_net_norm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.354054 kappadata-1.2.9/kappadata/common/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/copying/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/copying/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/copying/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/datasets/kd_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/loading/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/loading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/loading/image_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.358054 kappadata-1.2.9/kappadata/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/samplers/infinite_batch_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/samplers/interleaved_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/add_gaussian_noise_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/base/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_compose_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_identity_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_random_apply_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_scheduled_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_stochastic_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/base/kd_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/image_pos_embed_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/image_pos_embed_sincos.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_rand_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_rand_augment_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_color_jitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_erasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_horizontal_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_resized_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_random_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_rearrange.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_solarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/kd_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/norm/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/transforms/norm/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/base/kd_norm_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/kd_image_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/norm/kd_image_range_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchify_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchwise_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchwise_random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/patchwise_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/save_state_to_context_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/transforms/unpatchify_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/class_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/color_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/magnitude_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/multi_crop_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/param_checking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/pos_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/utils/transform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.366054 kappadata-1.2.9/kappadata/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/visualization/visualize_two_random_crop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/mode_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.370054 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-12 21:50:51.000000 kappadata-1.2.9/kappadata/wrappers/torch_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:53:00.346054 kappadata-1.2.9/kappadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 21:53:00.000000 kappadata-1.2.9/kappadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-12 21:50:51.000000 kappadata-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 21:53:00.370054 kappadata-1.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.146218 kappadata-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 07:59:05.000000 kappadata-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-03 08:01:28.146218 kappadata-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-03 07:59:05.000000 kappadata-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.110219 kappadata-1.3.0/kappadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 08:01:10.000000 kappadata-1.3.0/kappadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.110219 kappadata-1.3.0/kappadata/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/caching/cached_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/caching/shared_dict_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/collators/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/kd_collator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/kd_compose_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/base/kd_single_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/kd_mix_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/collators/pad_sequences_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/collators/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/collators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/collators/mae_finetune_mix_collator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/datasets/kd_image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.114219 kappadata-1.3.0/kappadata/common/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/byol_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/imagenet_minaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/imagenet_noaug_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/mae_finetune_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/common/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_ade20k_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_cifar100_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_cifar10_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/transforms/norm/kd_image_net_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/common/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/copying/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/copying/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/copying/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/copying/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/datasets/kd_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.118219 kappadata-1.3.0/kappadata/loading/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/loading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/loading/image_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.122218 kappadata-1.3.0/kappadata/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/distributed_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/infinite_batch_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/interleaved_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/semi_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/samplers/sequential_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.130219 kappadata-1.3.0/kappadata/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.130219 kappadata-1.3.0/kappadata/transforms/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_compose_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_identity_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_random_apply_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_scheduled_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_stochastic_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/base/kd_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/image_pos_embed_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/image_pos_embed_sincos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_columnwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_minsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_rand_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_rand_augment_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_additive_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_color_jitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_erasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_resized_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_random_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_rearrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_simple_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_solarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_three_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/kd_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.134219 kappadata-1.3.0/kappadata/transforms/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/kd_image_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/kd_image_range_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/norm/kd_norm_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchify_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchwise_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchwise_random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/patchwise_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/save_state_to_context_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.134219 kappadata-1.3.0/kappadata/transforms/semseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_random_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/semseg/kd_semseg_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/transforms/unpatchify_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.138218 kappadata-1.3.0/kappadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/class_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/color_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/getall_class_as_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/magnitude_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/multi_crop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/param_checking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/pos_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/utils/transform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.138218 kappadata-1.3.0/kappadata/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_dataset_imgsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_mae_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_masked_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/visualization/visualize_two_random_crop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.142218 kappadata-1.3.0/kappadata/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.142218 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/subset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/mode_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.146218 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.146218 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-03 07:59:05.000000 kappadata-1.3.0/kappadata/wrappers/torch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:01:28.110219 kappadata-1.3.0/kappadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 08:01:28.000000 kappadata-1.3.0/kappadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-03 07:59:05.000000 kappadata-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-03 08:01:28.146218 kappadata-1.3.0/setup.cfg
```

### Comparing `kappadata-1.2.9/LICENSE` & `kappadata-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/PKG-INFO` & `kappadata-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.2.9
+Version: 1.3.0
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 - various dataset filters and other dataset manipulation
     - filter by class
     - limit size to a %
     - [Mixup](https://arxiv.org/abs/1710.09412)
     - [Cutmix](https://arxiv.org/abs/1905.04899)
     - label smoothing
     - ...
+- repeated augmentations
 
 # Modular datasets
 
 [pytorch datasets](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) load all data in the `__getitem__`.
 KappaData decouples the `__getitem__` such that single properties of the dataset can be loaded independently.
 
 ## Image classification dataset example
```

### Comparing `kappadata-1.2.9/README.md` & `kappadata-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - various dataset filters and other dataset manipulation
     - filter by class
     - limit size to a %
     - [Mixup](https://arxiv.org/abs/1710.09412)
     - [Cutmix](https://arxiv.org/abs/1905.04899)
     - label smoothing
     - ...
+- repeated augmentations
 
 # Modular datasets
 
 [pytorch datasets](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) load all data in the `__getitem__`.
 KappaData decouples the `__getitem__` such that single properties of the dataset can be loaded independently.
 
 ## Image classification dataset example
```

### Comparing `kappadata-1.2.9/kappadata/caching/cached_dataset.py` & `kappadata-1.3.0/kappadata/caching/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/caching/shared_dict_dataset.py` & `kappadata-1.3.0/kappadata/caching/shared_dict_dataset.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/collators/base/kd_collator_base.py` & `kappadata-1.3.0/kappadata/collators/base/kd_collator_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/collators/base/kd_compose_collator.py` & `kappadata-1.3.0/kappadata/collators/base/kd_compose_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/collators/base/kd_single_collator.py` & `kappadata-1.3.0/kappadata/collators/base/kd_single_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/collators/kd_mix_collator.py` & `kappadata-1.3.0/kappadata/collators/kd_mix_collator.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,21 +83,27 @@
     @property
     def total_p(self) -> float:
         return self.mixup_p + self.cutmix_p
 
     def collate(self, batch, dataset_mode, ctx=None):
         # extract properties from batch
         idx, x, y = None, None, None
+        is_binary_classification = False
         if ModeWrapper.has_item(mode=dataset_mode, item="index"):
             idx = ModeWrapper.get_item(mode=dataset_mode, item="index", batch=batch)
         if ModeWrapper.has_item(mode=dataset_mode, item="x"):
             x = ModeWrapper.get_item(mode=dataset_mode, item="x", batch=batch)
         if ModeWrapper.has_item(mode=dataset_mode, item="class"):
             y = ModeWrapper.get_item(mode=dataset_mode, item="class", batch=batch).type(torch.float32)
-            assert y.ndim == 2, "KDMixCollator expects classes to be in one-hot format"
+            # y has to be 2d tensor of in one-hot format (multi-class) or 1d tensor (binary-classification)
+            if y.ndim != 2:
+                assert y.ndim == 1 and 0. <= y.min() and y.max() <= 1., \
+                    "KDMixCollator expects classes to be in one-hot format"
+                y = y.unsqueeze(1)
+                is_binary_classification = True
         batch_size = len(x)
 
         # sample apply
         if self.apply_mode == "batch":
             apply = torch.full(size=(batch_size,), fill_value=self.rng.random() < self.total_p)
         elif self.apply_mode == "sample":
             apply = torch.from_numpy(self.rng.random(batch_size)) < self.total_p
@@ -174,14 +180,16 @@
 
         # update properties in batch
         if idx is not None:
             batch = ModeWrapper.set_item(mode=dataset_mode, item="index", batch=batch, value=idx)
         if x is not None:
             batch = ModeWrapper.set_item(mode=dataset_mode, item="x", batch=batch, value=x)
         if y is not None:
+            if is_binary_classification:
+                y = y.squeeze(1)
             batch = ModeWrapper.set_item(mode=dataset_mode, item="class", batch=batch, value=y)
         return batch
 
     def get_random_bbox(self, h, w, lamb):
         n_bboxes = len(lamb)
         bbox_hcenter = torch.from_numpy(self.rng.integers(h, size=(n_bboxes,)))
         bbox_wcenter = torch.from_numpy(self.rng.integers(w, size=(n_bboxes,)))
@@ -197,14 +205,16 @@
         bbox = torch.stack([top, left, bot, right], dim=1)
 
         lamb_adjusted = 1.0 - (bot - top) * (right - left) / (h * w)
 
         return bbox, lamb_adjusted
 
     def shuffle(self, item, permutation):
+        if len(item) == 1:
+            return item.clone(), None
         if self.shuffle_mode == "roll":
             return item.roll(shifts=1, dims=0), None
         if self.shuffle_mode == "flip":
             assert len(item) % 2 == 0
             return item.flip(0), None
         if self.shuffle_mode == "random":
             if permutation is None:
```

### Comparing `kappadata-1.2.9/kappadata/collators/pad_sequences_collator.py` & `kappadata-1.3.0/kappadata/collators/pad_sequences_collator.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/datasets/kd_image_folder.py` & `kappadata-1.3.0/kappadata/common/datasets/kd_image_folder.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/transforms/byol_transforms.py` & `kappadata-1.3.0/kappadata/common/transforms/byol_transforms.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from kappadata.transforms.kd_gaussian_blur_pil import KDGaussianBlurPIL
 from kappadata.transforms.kd_random_color_jitter import KDRandomColorJitter
 from kappadata.transforms.kd_random_gaussian_blur_pil import KDRandomGaussianBlurPIL
 from kappadata.transforms.kd_random_grayscale import KDRandomGrayscale
 from kappadata.transforms.kd_random_horizontal_flip import KDRandomHorizontalFlip
 from kappadata.transforms.kd_random_resized_crop import KDRandomResizedCrop
 from kappadata.transforms.kd_random_solarize import KDRandomSolarize
+from kappadata.transforms.norm.kd_image_norm import KDImageNorm
 from .norm import string_to_norm
 from .norm.kd_image_net_norm import KDImageNetNorm
-from kappadata.transforms.norm.kd_image_norm import KDImageNorm
 
 
 class BYOLTransform(KDComposeTransform):
     def __init__(
             self,
             size=224,
             interpolation="bicubic",
```

### Comparing `kappadata-1.2.9/kappadata/common/transforms/imagenet_minaug_transforms.py` & `kappadata-1.3.0/kappadata/common/transforms/imagenet_minaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/transforms/imagenet_noaug_transforms.py` & `kappadata-1.3.0/kappadata/common/transforms/imagenet_noaug_transforms.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/transforms/mae_finetune_transform.py` & `kappadata-1.3.0/kappadata/common/transforms/mae_finetune_transform.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py` & `kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py` & `kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py` & `kappadata-1.3.0/kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/copying/image_folder.py` & `kappadata-1.3.0/kappadata/copying/image_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections import namedtuple
 from pathlib import Path
 
 import joblib
 
 from kappadata.utils.logging import log
 
-CopyImageFolderResult = namedtuple("CopyFolderResult", "was_copied was_deleted was_zip was_zip_classwise")
+CopyImageFolderResult = namedtuple("CopyImageFolderResult", "was_copied was_deleted was_zip was_zip_classwise")
 
 
 def _check_src_path(src_path):
     if src_path.exists() and src_path.is_dir():
         return True
     if src_path.with_suffix(".zip").exists():
         return True
```

### Comparing `kappadata-1.2.9/kappadata/datasets/kd_concat_dataset.py` & `kappadata-1.3.0/kappadata/datasets/kd_concat_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 
 from torch.utils.data import ConcatDataset
 
 from kappadata.errors import UseModeWrapperException
 
 
 class KDConcatDataset(ConcatDataset):
+    def __init__(self, *args, balanced_sampling=False, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.balanced_sampling = balanced_sampling
+
     def __getattr__(self, item):
         if item.startswith("getitem_"):
             # all methods starting with getitem_ are called with self.datasets[dataset_idx][sample_idx]
             return partial(self._call_getitem, item)
         if item == "datasets":
             return getattr(super(), item)
         if item.startswith("getall_"):
             # all methods starting with getall_ have to concatenate the result of dataset.getall_... for all datasets
             return partial(self._call_getall, item)
         # warning/exception here might make sense
         return getattr(self.datasets[0], item)
 
     def _call_getitem(self, item, idx, *args, **kwargs):
-        dataset_idx, sample_idx = self._to_concat_idx(idx)
+        if self.balanced_sampling:
+            dataset_idx = idx % len(self.datasets)
+            sample_idx = int(idx / len(self.datasets)) % len(self.datasets[dataset_idx])
+        else:
+            dataset_idx, sample_idx = self._to_concat_idx(idx)
         func = getattr(self.datasets[dataset_idx], item)
         return func(sample_idx, *args, **kwargs)
 
     def _call_getall(self, item):
         result = []
         for dataset in self.datasets:
             dataset_result = getattr(dataset, item)()
@@ -61,14 +69,25 @@
     @property
     def root_dataset(self):
         if len(self.datasets) == 1:
             return self.datasets[0].root_dataset
         # warning/exception here might make sense
         return self.datasets[0].root_dataset
 
+    @property
+    def fused_operations(self):
+        if len(self.datasets) == 1:
+            return self.datasets[0].fused_operations
+        # warning/exception here might make sense
+        return self.datasets[0].fused_operations
+
+    @property
+    def requires_propagate_ctx(self):
+        return any(ds.requires_propagate_ctx for ds in self.datasets)
+
     def has_wrapper(self, wrapper):
         if len(self.datasets) == 1:
             return self.datasets[0].has_wrapper(wrapper)
         # warning/exception here might make sense
         return self.datasets[0].has_wrapper(wrapper)
 
     def has_wrapper_type(self, wrapper_type):
@@ -106,7 +125,11 @@
 
     def worker_init_fn(self, rank, **kwargs):
         for dataset in self.datasets:
             dataset.worker_init_fn(rank, **kwargs)
 
     def __getitem__(self, idx):
         raise UseModeWrapperException
+
+    def __len__(self):
+        assert not self.balanced_sampling
+        return super().__len__()
```

### Comparing `kappadata-1.2.9/kappadata/datasets/kd_dataset.py` & `kappadata-1.3.0/kappadata/datasets/kd_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
+from functools import partial
 
 from torch.utils.data import Dataset
 
-from kappadata.errors import UseModeWrapperException
 from kappadata.error_messages import getshape_instead_of_getdim
-from functools import partial
+from kappadata.errors import UseModeWrapperException
 
 
 class KDDataset(Dataset):
     def __init__(self):
         super().__init__()
         self.logger = logging.getLogger(type(self).__name__)
 
@@ -35,14 +35,22 @@
         """ release resources occupied by dataset (e.g. filehandles) """
         pass
 
     @property
     def root_dataset(self):
         return self
 
+    @property
+    def fused_operations(self):
+        return []
+
+    @property
+    def requires_propagate_ctx(self):
+        return False
+
     @staticmethod
     def has_wrapper(wrapper):
         return False
 
     @staticmethod
     def has_wrapper_type(wrapper_type):
         return False
```

### Comparing `kappadata-1.2.9/kappadata/datasets/kd_subset.py` & `kappadata-1.3.0/kappadata/datasets/kd_subset.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,22 @@
     def __exit__(self, *_):
         self.dispose()
 
     @property
     def root_dataset(self):
         return self.dataset.root_dataset
 
+    @property
+    def fused_operations(self):
+        return self.dataset.fused_operations
+
+    @property
+    def requires_propagate_ctx(self):
+        return self.dataset.requires_propagate_ctx
+
     def has_wrapper(self, wrapper):
         if self == wrapper:
             return True
         return self.dataset.has_wrapper(wrapper)
 
     def has_wrapper_type(self, wrapper_type):
         if type(self) == wrapper_type:
```

### Comparing `kappadata-1.2.9/kappadata/datasets/kd_wrapper.py` & `kappadata-1.3.0/kappadata/datasets/kd_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,22 @@
         self.dataset.dispose()
 
     @property
     def root_dataset(self):
         # KDDataset implements root_dataset -> __getitem__ doesn't trigger
         return self.dataset.root_dataset
 
+    @property
+    def fused_operations(self):
+        return self.dataset.fused_operations
+
+    @property
+    def requires_propagate_ctx(self):
+        return self.dataset.requires_propagate_ctx
+
     def has_wrapper(self, wrapper):
         if self == wrapper:
             return True
         return self.dataset.has_wrapper(wrapper)
 
     def has_wrapper_type(self, wrapper_type):
         if type(self) == wrapper_type:
```

### Comparing `kappadata-1.2.9/kappadata/error_messages.py` & `kappadata-1.3.0/kappadata/error_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 def getshape_instead_of_getdim(getdim_names):
     getshape_names = [f"getshape_{getdim_name[len('getdim_'):]}" for getdim_name in getdim_names]
     return f"implement 'getshape' instead of 'getdim' (expected {getshape_names} but found {getdim_names})"
 
+
 def too_little_samples_for_class(class_idx, actual, expected):
     return f"class {class_idx} has only {actual} samples (requires at least {expected} samples)"
 
 
 KD_MIX_WRAPPER_REQUIRES_SEED_OR_CONTEXT = (
     "KDMixWrapper requires either a context or a seed to ensure same mixing of samples and labels "
     "(NOTE: using a seed will additionally make the transform deterministc per sample)"
```

### Comparing `kappadata-1.2.9/kappadata/factory.py` & `kappadata-1.3.0/kappadata/factory.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/samplers/infinite_batch_sampler.py` & `kappadata-1.3.0/kappadata/samplers/infinite_batch_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.samples = samples
 
     def __iter__(self):
         epochs = 0
         updates = 0
         samples = 0
         while True:
-            if isinstance(self.sampler, DistributedSampler):
+            if hasattr(self.sampler, "set_epoch"):
                 self.sampler.set_epoch(epochs)
             for batch in super().__iter__():
                 updates += 1
                 samples += len(batch)
                 yield batch
             epochs += 1
             if (
```

### Comparing `kappadata-1.2.9/kappadata/samplers/interleaved_sampler.py` & `kappadata-1.3.0/kappadata/samplers/interleaved_sampler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import bisect
-from torch.utils.data import default_collate, DataLoader
 from dataclasses import dataclass
 
 from torch.utils.data import ConcatDataset, DistributedSampler
+from torch.utils.data import default_collate, DataLoader
 
 
 @dataclass
 class InterleavedSamplerConfig:
     sampler: object
     every_n_epochs: int = None
     every_n_updates: int = None
@@ -20,143 +20,231 @@
         if self.every_n_updates is not None:
             interval_strs.append(f"every_n_updates={self.every_n_updates}")
         if self.every_n_samples is not None:
             interval_strs.append(f"every_n_samples={self.every_n_samples}")
         return f"{type(self).__name__}({','.join(interval_strs)})"
 
 
+# can't be a local class as it is required to be pickleable
+# AttributeError: Can't pickle local object 'InterleavedSampler.__init__.<locals>._InterleavedConcatDataset'
+class _InterleavedConcatDataset(ConcatDataset):
+    """ same as ConcatDataset but it returns the dataset index """
+
+    def __getitem__(self, idx):
+        if idx < 0:
+            if -idx > len(self):
+                raise ValueError("absolute value of index should not exceed dataset length")
+            idx = len(self) + idx
+        dataset_idx = bisect.bisect_right(self.cumulative_sizes, idx)
+        if dataset_idx == 0:
+            sample_idx = idx
+        else:
+            sample_idx = idx - self.cumulative_sizes[dataset_idx - 1]
+        return dataset_idx, self.datasets[dataset_idx][sample_idx]
+
+    def worker_init_fn(self, rank, **kwargs):
+        for dataset in self.datasets:
+            dataset.worker_init_fn(rank, dataset_len=len(dataset), **kwargs)
+
+
+# can't be a local class as it is required to be pickleable
+# AttributeError: Can't pickle local object 'InterleavedSampler.__init__.<locals>._InterleavedCollator'
+class _InterleavedCollator:
+    def __init__(self, collators):
+        self.collators = collators
+
+    def __call__(self, data):
+        dataset_idxs, data = zip(*data)
+        assert all(dataset_idxs[0] == idx for idx in dataset_idxs)
+        return self.collators[dataset_idxs[0]](data)
+
+
+# can't be a local class as it is required to be pickleable
+# AttributeError: Can't pickle local object 'InterleavedSampler.__init__.<locals>._InterleavedBatchSampler'
+class _InterleavedBatchSampler:
+    def __init__(self, sampler):
+        super().__init__()
+        self.sampler = sampler
+
+    def __iter__(self):
+        idxs = []
+        for is_full_batch, idx in self.sampler:
+            idxs.append(idx)
+            if is_full_batch:
+                yield idxs
+                idxs = []
+        assert len(idxs) == 0
+
+    def __len__(self):
+        raise NotImplementedError
+
+
 class InterleavedSampler:
     def __init__(
             self,
             main_sampler,
             batch_size,
             configs=None,
             # properties of main sampler
             drop_last=True,
             main_collator=None,
             # duration of InterleavedSampler
             epochs=None,
             updates=None,
             samples=None,
+            start_epoch=None,
+            start_update=None,
+            start_sample=None,
+            # batch_size used for dropping last batch
+            drop_last_batch_size=None,
     ):
         super().__init__()
         assert isinstance(batch_size, int) and 0 < batch_size
         assert batch_size <= len(main_sampler)
-        assert epochs is None or (isinstance(epochs, int) and 0 < epochs)
-        assert updates is None or (isinstance(updates, int) and 0 < updates)
-        assert samples is None or (isinstance(samples, int) and 0 < samples)
-        assert sum([epochs is not None, updates is not None, samples is not None]) <= 1
+        if drop_last_batch_size is not None:
+            assert drop_last and drop_last_batch_size % batch_size == 0
+            assert isinstance(drop_last_batch_size, int) and batch_size <= drop_last_batch_size
+            assert drop_last_batch_size <= len(main_sampler)
+        assert epochs is None or (isinstance(epochs, int) and 0 <= epochs)
+        assert updates is None or (isinstance(updates, int) and 0 <= updates)
+        assert samples is None or (isinstance(samples, int) and 0 <= samples)
+        assert sum([epochs is not None, updates is not None, samples is not None]) == 1
         configs = configs or []
         for config in configs:
             assert (
                     (config.every_n_epochs is not None) or
                     (config.every_n_updates is not None) or
                     (config.every_n_samples is not None)
             )
             assert config.every_n_epochs is None or 0 < config.every_n_epochs
             assert config.every_n_updates is None or 0 < config.every_n_updates
             assert config.every_n_samples is None or 0 < config.every_n_samples
 
+        # infer full start checkpoint from one of epoch/update/sample
+        if start_epoch is not None:
+            assert isinstance(start_epoch, int) and start_update is None and start_sample is None
+            start_update = len(main_sampler) // batch_size * start_epoch
+            start_sample = start_update * batch_size
+        elif start_update is not None:
+            assert start_epoch is None and isinstance(start_update, int) and start_sample is None
+            start_epoch = int(start_update / (len(main_sampler) // batch_size))
+            start_sample = start_update * batch_size
+            if start_update % (len(main_sampler) // batch_size) != 0 or not drop_last:
+                raise NotImplementedError("defining start_update would require to skip forward in the sampler")
+        elif start_sample is not None:
+            assert start_epoch is None and start_update is None and isinstance(start_sample, int)
+            assert start_sample % batch_size == 0
+            start_update = start_sample // batch_size
+            start_epoch = int(start_update / (len(main_sampler) // batch_size))
+            if start_update % (len(main_sampler) // batch_size) != 0 or not drop_last:
+                raise NotImplementedError("defining start_update would require to skip forward in the sampler")
+        else:
+            start_epoch = start_update = start_sample = 0
+
         self.main_sampler = main_sampler
         self.drop_last = drop_last
         self.configs = configs
         self.batch_size = batch_size
         self.epochs = epochs
         self.updates = updates
         self.samples = samples
+        self.start_epoch = start_epoch
+        self.start_update = start_update
+        self.start_sample = start_sample
+        self.drop_last_batch_size = drop_last_batch_size
 
         def _get_data_source(sampler):
             if hasattr(sampler, "data_source"):
                 return sampler.data_source
             if hasattr(sampler, "dataset"):
                 return sampler.dataset
             raise NotImplementedError
 
         self.index_offsets = [len(_get_data_source(self.main_sampler))]
         for config in self.configs[:-1]:
             self.index_offsets.append(self.index_offsets[-1] + len(_get_data_source(config.sampler)))
 
-
-        class InterleavedConcatDataset(ConcatDataset):
-            """ same as ConcatDataset but it returns the dataset index """
-            def __getitem__(self, idx):
-                if idx < 0:
-                    if -idx > len(self):
-                        raise ValueError("absolute value of index should not exceed dataset length")
-                    idx = len(self) + idx
-                dataset_idx = bisect.bisect_right(self.cumulative_sizes, idx)
-                if dataset_idx == 0:
-                    sample_idx = idx
-                else:
-                    sample_idx = idx - self.cumulative_sizes[dataset_idx - 1]
-                return dataset_idx, self.datasets[dataset_idx][sample_idx]
-
-        self.dataset = InterleavedConcatDataset(
+        self.dataset = _InterleavedConcatDataset(
             [_get_data_source(self.main_sampler)] +
             [_get_data_source(config.sampler) for config in self.configs]
         )
 
-        class InterleavedCollator:
-            def __init__(self, collators):
-                self.collators = collators
-
-            def __call__(self, data):
-                dataset_idxs, data = zip(*data)
-                assert all(dataset_idxs[0] == idx for idx in dataset_idxs)
-                return self.collators[dataset_idxs[0]](data)
-
-        self.collator = InterleavedCollator(
+        self.collator = _InterleavedCollator(
             [main_collator or default_collate] +
             [config.collator or default_collate for config in self.configs]
         )
 
-        class InterleavedBatchSampler:
-            def __init__(self, sampler):
-                super().__init__()
-                self.sampler = sampler
-
-            def __iter__(self):
-                idxs = []
-                for is_full_batch, idx in self.sampler:
-                    idxs.append(idx)
-                    if is_full_batch:
-                        yield idxs
-                        idxs = []
-                assert len(idxs) == 0
-
-            def __len__(self):
-                raise NotImplementedError
+        self.batch_sampler = _InterleavedBatchSampler(self)
 
-        self.batch_sampler = InterleavedBatchSampler(self)
-
-    def get_data_loader(self, num_workers: int = 0, pin_memory: bool = False) -> DataLoader:
+    def get_data_loader(
+            self,
+            num_workers: int = 0,
+            pin_memory: bool = False,
+            prefetch_factor: int = None,
+            worker_init_fn = None,
+    ) -> DataLoader:
+        # the default value of prefetch_factor changed from 2 to None in pytorch 2.0 -> pass via optional kwarg
+        kwargs = {}
+        if num_workers > 0 and prefetch_factor is not None:
+            kwargs["prefetch_factor"] = prefetch_factor
         return DataLoader(
             dataset=self.dataset,
             batch_sampler=self.batch_sampler,
             collate_fn=self.collator,
             num_workers=num_workers,
             pin_memory=pin_memory,
+            worker_init_fn=worker_init_fn,
+            **kwargs,
         )
 
     def __iter__(self):
+        if self.epochs == 0 or self.updates == 0 or self.samples == 0:
+            assert self.start_epoch == 0 and self.start_update == 0 and self.start_sample == 0
+            yield from self._eval_loop()
+        else:
+            yield from self._training_loop()
+
+    def _eval_loop(self):
+        for config_idx, config in enumerate(self.configs):
+            index_offset = self.index_offsets[config_idx]
+            sample_in_interleaved = 0
+            for interleaved_idx in config.sampler:
+                sample_in_interleaved += 1
+                if (
+                        sample_in_interleaved % self.batch_size == 0 or
+                        sample_in_interleaved == len(config.sampler)
+                ):
+                    yield True, index_offset + interleaved_idx
+                else:
+                    yield False, index_offset + interleaved_idx
+
+    def _training_loop(self):
         if self.drop_last:
-            if len(self.main_sampler) < self.batch_size:
-                self.batch_size = len(self.main_sampler)
-            samples_per_epoch = len(self.main_sampler) // self.batch_size * self.batch_size
+            if self.drop_last_batch_size is not None:
+                if len(self.main_sampler) < self.drop_last_batch_size:
+                    factor = self.drop_last_batch_size // self.batch_size
+                    self.drop_last_batch_size = len(self.main_sampler) - len(self.main_sampler) % factor
+                    self.batch_size = self.drop_last_batch_size // factor
+                batch_size = self.drop_last_batch_size
+            else:
+                if len(self.main_sampler) < self.batch_size:
+                    self.batch_size = len(self.main_sampler)
+                batch_size = self.batch_size
+            samples_per_epoch = len(self.main_sampler) // batch_size * batch_size
         else:
             samples_per_epoch = len(self.main_sampler)
 
-        sample = 0
-        epoch = 0
-        update = 0
+        epoch = self.start_epoch
+        update = self.start_update
+        sample = self.start_sample
         sample_in_update = 0
         sample_at_last_update = 0
         while True:
             sample_in_epoch = 0
-            if isinstance(self.main_sampler, DistributedSampler):
+            if hasattr(self.main_sampler, "set_epoch"):
                 self.main_sampler.set_epoch(epoch)
             for main_idx in self.main_sampler:
                 sample += 1
                 sample_in_epoch += 1
                 sample_in_update += 1
                 if sample_in_update == self.batch_size or sample_in_epoch == samples_per_epoch:
                     yield True, main_idx
```

### Comparing `kappadata-1.2.9/kappadata/transforms/__init__.py` & `kappadata-1.3.0/kappadata/transforms/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-# augs
-from .add_gaussian_noise_transform import AddGaussianNoiseTransform
-# base
-from .base import KDComposeTransform
-from .base import KDIdentityTransform
-from .base import KDScheduledTransform
-from .base import KDStochasticTransform
-from .base import KDTransform
-# augs
+from .kd_additive_gaussian_noise import KDAdditiveGaussianNoise
+from .base import *
 from .image_pos_embed_grid import ImagePosEmbedGrid
 from .image_pos_embed_sincos import ImagePosEmbedSincos
 from .kd_bucketize import KDBucketize
-#
 from .kd_color_jitter import KDColorJitter
+from .kd_horizontal_flip import KDHorizontalFlip
+from .kd_columnwise_norm import KDColumnwiseNorm
 from .kd_gaussian_blur_pil import KDGaussianBlurPIL
 from .kd_gaussian_blur_tv import KDGaussianBlurTV
+from .kd_grayscale import KDGrayscale
+from .kd_minsize import KDMinsize
 from .kd_rand_augment import KDRandAugment
 from .kd_rand_augment_custom import KDRandAugmentCustom
 from .kd_random_apply import KDRandomApply
 from .kd_random_color_jitter import KDRandomColorJitter
 from .kd_random_crop import KDRandomCrop
 from .kd_random_erasing import KDRandomErasing
 from .kd_random_gaussian_blur_pil import KDRandomGaussianBlurPIL
 from .kd_random_gaussian_blur_tv import KDRandomGaussianBlurTV
 from .kd_random_grayscale import KDRandomGrayscale
 from .kd_random_horizontal_flip import KDRandomHorizontalFlip
 from .kd_random_resized_crop import KDRandomResizedCrop
 from .kd_random_solarize import KDRandomSolarize
 from .kd_rearrange import KDRearrange
 from .kd_resize import KDResize
+from .kd_simple_random_crop import KDSimpleRandomCrop
 from .kd_solarize import KDSolarize
-# norm
-from .norm.kd_image_norm import KDImageNorm
-from .norm.kd_image_range_norm import KDImageRangeNorm
-#
+from .kd_three_augment import KDThreeAugment
+from .kd_threshold import KDThreshold
+from .norm import *
 from .patchify_image import PatchifyImage
 from .patchwise_norm import PatchwiseNorm
 from .patchwise_random_rotation import PatchwiseRandomRotation
 from .patchwise_shuffle import PatchwiseShuffle
 from .save_state_to_context_transform import SaveStateToContextTransform
+from .semseg import *
 from .unpatchify_image import UnpatchifyImage
+from .kd_random_additive_gaussian_noise import KDRandomAdditiveGaussianNoise
+from .kd_random_threshold import KDRandomThreshold
```

### Comparing `kappadata-1.2.9/kappadata/transforms/add_gaussian_noise_transform.py` & `kappadata-1.3.0/kappadata/transforms/kd_additive_gaussian_noise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 import torch
 
 from kappadata.utils.magnitude_sampler import MagnitudeSampler
 from .base.kd_stochastic_transform import KDStochasticTransform
 
 
-class AddGaussianNoiseTransform(KDStochasticTransform):
+class KDAdditiveGaussianNoise(KDStochasticTransform):
     def __init__(
             self,
+            std: float,
             magnitude: float = 1.,
             magnitude_std: float = float("inf"),
             magnitude_min: float = 0.,
             magnitude_max: float = 1.,
+            clip_min: float = None,
+            clip_max: float = None,
             **kwargs,
     ):
         super().__init__(**kwargs)
+        self.std = std
         self.magnitude_sampler = MagnitudeSampler(
             magnitude=magnitude,
             magnitude_std=magnitude_std,
             magnitude_min=magnitude_min,
             magnitude_max=magnitude_max,
         )
         self.ctx_key = f"{self.ctx_prefix}.magnitude"
+        self.clip_min = clip_min
+        self.clip_max = clip_max
+
+    def _gauss_noise(self, x, magnitude):
+        return
 
     def _scale_strength(self, factor):
         self.magnitude_sampler.scale_strength(factor)
 
     def __call__(self, x, ctx=None):
         magnitude = self.magnitude_sampler.sample(self.rng)
-        noise = torch.from_numpy(self.rng.normal(scale=magnitude, size=x.shape)).float()
+        noise = torch.from_numpy(self.rng.normal(scale=magnitude * self.std, size=x.shape)).float()
         if ctx is not None:
             ctx[self.ctx_key] = magnitude
-        return x + noise
+        x = x + noise
+        if self.clip_min is not None or self.clip_max is not None:
+            x = torch.clamp(x, self.clip_min, self.clip_max)
+        return x
```

### Comparing `kappadata-1.2.9/kappadata/transforms/base/kd_compose_transform.py` & `kappadata-1.3.0/kappadata/transforms/base/kd_compose_transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 
 
 class KDComposeTransform(KDTransform):
     def __init__(self, transforms):
         super().__init__()
         self.transforms = [object_to_transform(transform) for transform in transforms]
 
+    def _worker_init_fn(self, rank, num_workers, **kwargs):
+        for t in self.transforms:
+            # noinspection PyProtectedMember
+            t._worker_init_fn(rank, num_workers, **kwargs)
+
+    @property
+    def is_deterministic(self):
+        return all(t.is_deterministic for t in self.transforms)
+
+    @property
+    def is_kd_transform(self):
+        return all(isinstance(t, KDTransform))
+
     def __call__(self, x, ctx=None):
         if ctx is None:
             ctx = {}
         for t in self.transforms:
             if isinstance(x, (list, tuple)):
                 # apply for each sample
                 x = [self._apply(t, xx, ctx) for xx in x]
```

### Comparing `kappadata-1.2.9/kappadata/transforms/base/kd_random_apply_base.py` & `kappadata-1.3.0/kappadata/transforms/base/kd_random_apply_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/base/kd_scheduled_transform.py` & `kappadata-1.3.0/kappadata/transforms/base/kd_scheduled_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from kappaschedules import LinearIncreasingSchedule, object_to_schedule
 
+import torch
 from kappadata.factory import object_to_transform
 from .kd_transform import KDTransform
 
 
 class KDScheduledTransform(KDTransform):
     def __init__(self, transform, schedule=None):
         super().__init__()
@@ -18,15 +19,16 @@
         self.schedule = object_to_schedule(schedule) or LinearIncreasingSchedule()
 
     def _worker_init_fn(
             self,
             rank,
             num_workers,
             batch_size=None,
-            dataset_length=None,
+            dataset_len=None,
+            world_size=None,
             drop_last=None,
             epochs=None,
             updates=None,
             samples=None,
             **__,
     ):
         self.rank = rank
@@ -34,20 +36,22 @@
         assert batch_size is not None
         self.batch_size = batch_size
 
         # calculate total_n_batches (number of batches independent of num_workers)
         if epochs is not None:
             assert updates is None and samples is None
             assert drop_last is not None
-            assert dataset_length is not None
+            assert dataset_len is not None
+            assert world_size is not None
             assert isinstance(epochs, int) and epochs >= 0
+            dataset_len //= world_size
             if drop_last:
-                batches_per_epoch = dataset_length // batch_size
+                batches_per_epoch = dataset_len // batch_size
             else:
-                batches_per_epoch = (dataset_length + batch_size - 1) // batch_size
+                batches_per_epoch = (dataset_len + batch_size - 1) // batch_size
             self.n_batches = epochs * batches_per_epoch
         elif updates is not None:
             assert samples is None
             assert isinstance(updates, int) and updates >= 0
             self.n_batches = updates
         elif samples is not None:
             assert isinstance(samples, int) and samples >= 0
@@ -55,18 +59,18 @@
                 self.n_batches = samples // batch_size
             else:
                 self.n_batches = samples // batch_size + 1
         else:
             raise NotImplementedError
 
     def __call__(self, x, ctx=None):
-        # ideally this would be checked here, but this prohibits and call to the dataset outside the DataLoader loop
-        # right now it is up to the user to make sure that worker_init_fn is called
-        # assert self.n_batches is not None, "call KDScheduledTransform.worker_init_fn before applying the transform"
-
+        # make sure that worker_init_fn was called
+        if torch.utils.data.get_worker_info() is not None:
+            assert self.n_batches is not None, "call KDScheduledTransform.worker_init_fn before applying the transform"
+        # scale_strength when called in worker process
         if self.n_batches is not None:
             # caulculate progress
             batch_idx = self.sample_counter // self.batch_size * self.num_workers + self.rank
             strength = self.schedule.get_value(batch_idx, self.n_batches)
             self.sample_counter += 1
 
             # scale
```

### Comparing `kappadata-1.2.9/kappadata/transforms/base/kd_transform.py` & `kappadata-1.3.0/kappadata/transforms/base/kd_transform.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,32 @@
 class KDTransform:
     def __init__(self, ctx_prefix: str = None):
         self.ctx_prefix = ctx_prefix or type(self).__name__
         # sanity check to avoid accidentally overwriting base method
         assert type(self).scale_strength == KDTransform.scale_strength
         assert type(self).worker_init_fn == KDTransform.worker_init_fn
 
+    @property
+    def is_deterministic(self):
+        return True
+
+    def set_rng(self, rng):
+        pass
+
+    @property
+    def is_kd_transform(self):
+        return True
+
     def __call__(self, x, ctx=None):
         raise NotImplementedError
 
     def worker_init_fn(self, rank, **kwargs):
         # if num_workers == 0 -> get_worker_info() is None
-        # if num_workers the worker_init_fn can be called manually  although this is not recommended
-        # e.g. the counter of  a scheduled transform will be a global object and therefore no longer be correct
+        # if num_workers the worker_init_fn can be called manually although this is not recommended
+        # e.g. the counter of a scheduled transform will be a global object and therefore no longer be correct
         info = get_worker_info()
         if info is None:
             num_workers = 1
         else:
             num_workers = info.num_workers
         self._worker_init_fn(rank, num_workers, **kwargs)
```

### Comparing `kappadata-1.2.9/kappadata/transforms/image_pos_embed_grid.py` & `kappadata-1.3.0/kappadata/transforms/image_pos_embed_grid.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/image_pos_embed_sincos.py` & `kappadata-1.3.0/kappadata/transforms/image_pos_embed_sincos.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_bucketize.py` & `kappadata-1.3.0/kappadata/transforms/kd_bucketize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_color_jitter.py` & `kappadata-1.3.0/kappadata/transforms/kd_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_pil.py` & `kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_gaussian_blur_tv.py` & `kappadata-1.3.0/kappadata/transforms/kd_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_rand_augment.py` & `kappadata-1.3.0/kappadata/transforms/kd_rand_augment.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_color_jitter.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_color_jitter.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_crop.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_erasing.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_erasing.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_pil.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_pil.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_gaussian_blur_tv.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_gaussian_blur_tv.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_grayscale.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_grayscale.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,9 +10,8 @@
 
     def _scale_strength(self, factor):
         self.p = self.og_p * factor
 
     def forward(self, x, ctx):
         # if ctx is not None:
         #     ctx["random_grayscale"] = True
-        num_output_channels = F.get_image_num_channels(x)
-        return F.rgb_to_grayscale(x, num_output_channels=num_output_channels)
+        return F.rgb_to_grayscale(x, num_output_channels=F.get_image_num_channels(x))
```

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_resized_crop.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_rotation.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_random_solarize.py` & `kappadata-1.3.0/kappadata/transforms/kd_random_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_resize.py` & `kappadata-1.3.0/kappadata/transforms/kd_resize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_solarize.py` & `kappadata-1.3.0/kappadata/transforms/kd_solarize.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/kd_two_random_crop.py` & `kappadata-1.3.0/kappadata/transforms/kd_two_random_crop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from torchvision.transforms.functional import get_image_size, pad, crop
+from torchvision.transforms.functional import get_image_size, crop
 
-from kappadata.utils.param_checking import to_2tuple
-from .kd_random_crop import KDRandomCrop
 from kappadata.utils.bounding_box_utils import intersection_area_ijkl
+from .kd_random_crop import KDRandomCrop
 
 
 class KDTwoRandomCrop(KDRandomCrop):
     def __init__(self, *args, overlap_min=None, overlap_max=None, tries=20, **kwargs):
         super().__init__(*args, **kwargs)
         overlap_min = overlap_min or 0.
         overlap_max = overlap_max or 1.
@@ -14,19 +13,19 @@
         assert 0. <= overlap_max <= 1., overlap_max
         self.overlap_min = overlap_min
         self.overlap_max = overlap_max
         self.tries = tries
 
     def __call__(self, img, ctx=None):
         img = self._pad_image(img)
-        
+
         # make initial crop
         i0, j0, h0, w0 = self.get_params(img)
         crop0 = crop(img, i0, j0, h0, w0)
-        
+
         # make second crop
         out_of_tries = False
         k0 = i0 + h0
         l0 = j0 + w0
         area0 = h0 * w0
         tries = 0
         while True:
```

### Comparing `kappadata-1.2.9/kappadata/transforms/norm/base/kd_norm_base.py` & `kappadata-1.3.0/kappadata/transforms/norm/kd_norm_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/norm/kd_image_norm.py` & `kappadata-1.3.0/kappadata/transforms/norm/kd_image_norm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torchvision.transforms.functional import to_tensor, normalize
 
-from .base.kd_norm_base import KDNormBase
+from .kd_norm_base import KDNormBase
 
 
 class KDImageNorm(KDNormBase):
     def __init__(self, mean, std, **kwargs):
         super().__init__(**kwargs)
         assert len(mean) == len(std)
         self.mean = mean
```

### Comparing `kappadata-1.2.9/kappadata/transforms/norm/kd_image_range_norm.py` & `kappadata-1.3.0/kappadata/transforms/norm/kd_image_range_norm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torchvision.transforms.functional import to_tensor, normalize
 
-from .base.kd_norm_base import KDNormBase
+from .kd_norm_base import KDNormBase
 
 
 class KDImageRangeNorm(KDNormBase):
     def normalize(self, x, inplace=True):
         if not torch.is_tensor(x):
             x = to_tensor(x)
         n_channels = x.size(0)
```

### Comparing `kappadata-1.2.9/kappadata/transforms/patchify_image.py` & `kappadata-1.3.0/kappadata/transforms/patchify_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/patchwise_norm.py` & `kappadata-1.3.0/kappadata/transforms/patchwise_norm.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/transforms/patchwise_random_rotation.py` & `kappadata-1.3.0/kappadata/transforms/patchwise_random_rotation.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/utils/bounding_box_utils.py` & `kappadata-1.3.0/kappadata/utils/bounding_box_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-
-
 def intersection_area_ijkl(i0, j0, k0, l0, i1, j1, k1, l1):
     # i/j: coordinates of top left corner
     # k/l: coordinates of bottom right corner
     intersection_height = max(0, min(k0, k1) - max(i0, i1))
     intersection_width = max(0, min(l0, l1) - max(j0, j1))
     return intersection_height * intersection_width
 
+
 def intersection_area_ijhw(i0, j0, h0, w0, i1, j1, h1, w1):
     # i/j: coordinates of top left corner
     # h/w: height/width
     intersection_height = max(0, min(i0 + h0, i1 + h1) - max(i0, i1))
     intersection_width = max(0, min(j0 + w0, j1 + w1) - max(j0, j1))
     return intersection_height * intersection_width
-
```

### Comparing `kappadata-1.2.9/kappadata/utils/class_counts.py` & `kappadata-1.3.0/kappadata/utils/class_counts.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,33 @@
 
     # torch has much better asymptotic complexity (noticable from 1e9)
     if not torch.is_tensor(classes):
         if isinstance(classes, np.ndarray):
             classes = torch.from_numpy(classes).long()
         else:
             classes = torch.tensor(classes, dtype=torch.long)
+    # count unlabeled classes
+    unlabeled_count = (classes == -1).sum().item()
+    # filter out unlabeled
+    classes = classes[classes != -1]
+    assert torch.all(0 <= classes) and torch.all(classes < n_classes)
+
     # it is much faster on GPU, but also requires a lot of memory for large numbers
     counts = torch.zeros(n_classes, dtype=torch.long)
     unique_classes, unique_counts = classes.unique(return_counts=True)
     counts[unique_classes] = unique_counts
-    return counts
+    return counts, unlabeled_count
 
 
 def get_class_counts_from_dataset(dataset):
     classes = [dataset.getitem_class(i) for i in range(len(dataset))]
     return get_class_counts(classes=classes, n_classes=dataset.getdim_class())
 
 
 def get_class_counts_and_indices(dataset):
     # TODO inefficient implementation (e.g. https://stackoverflow.com/questions/30003068/how-to-get-a-list-of-all-indices-of-repeated-elements-in-a-numpy-array)
     classes = np.array([dataset.getitem_class(i) for i in range(len(dataset))])
-    counts = get_class_counts(classes=classes, n_classes=dataset.getdim_class())
+    counts, _ = get_class_counts(classes=classes, n_classes=dataset.getdim_class())
     indices = []
     for i in range(dataset.getdim_class()):
         indices.append((classes == i).nonzero()[0])
     return counts, indices
```

### Comparing `kappadata-1.2.9/kappadata/utils/color_histogram.py` & `kappadata-1.3.0/kappadata/utils/color_histogram.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/utils/magnitude_sampler.py` & `kappadata-1.3.0/kappadata/utils/magnitude_sampler.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/utils/multi_crop_utils.py` & `kappadata-1.3.0/kappadata/utils/multi_crop_utils.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/utils/pos_embed.py` & `kappadata-1.3.0/kappadata/utils/pos_embed.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/utils/save_image.py` & `kappadata-1.3.0/kappadata/utils/save_image.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/utils/transform_utils.py` & `kappadata-1.3.0/kappadata/utils/transform_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import partial
 
 from torchvision.transforms import Compose
 from torchvision.transforms import Normalize
 
-from kappadata import KDScheduledTransform
-from kappadata.transforms.base.kd_compose_transform import KDComposeTransform
-from kappadata.transforms.norm.base.kd_norm_base import KDNormBase
+from kappadata.transforms import KDScheduledTransform, KDComposeTransform
+from kappadata.transforms.norm.kd_norm_base import KDNormBase
 from kappadata.wrappers.sample_wrappers import XTransformWrapper
 
 
 def flatten_transform(transform):
     if transform is None:
         return []
     if isinstance(transform, KDScheduledTransform):
```

### Comparing `kappadata-1.2.9/kappadata/visualization/visualize_two_random_crop.py` & `kappadata-1.3.0/kappadata/visualization/visualize_two_random_crop.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import torch
-from kappadata.transforms.kd_two_random_crop import KDTwoRandomCrop
 from torchvision.transforms.functional import to_tensor, to_pil_image
 
+
 def visualize_two_random_crop(img, transform):
     if not torch.is_tensor(img):
         img = to_tensor(img)
     assert img.ndim == 3
-    
+
     ctx = {}
     _ = transform(img, ctx=ctx)
     ctx = ctx["two_random_crop"]
     i0, j0, h0, w0 = ctx["i0"], ctx["j0"], ctx["h0"], ctx["w0"]
     i1, j1, h1, w1 = ctx["i1"], ctx["j1"], ctx["h1"], ctx["w1"]
 
     mask = torch.zeros(*img.shape[1:], device=img.device)
     mask[i0:i0 + h0, j0:j0 + w0] = 1
     mask[i1:i1 + h1, j1:j1 + w1] = 1
 
-    return to_pil_image(img * mask), ctx["out_of_tries"]
+    return to_pil_image(img * mask), ctx["out_of_tries"]
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         # check params and make unique
         self._check_params(valid_classes=valid_classes, invalid_classes=invalid_classes)
         self.valid_classes = set(valid_classes) if valid_classes is not None else None
         self.invalid_classes = set(invalid_classes) if invalid_classes is not None else None
 
         # use numpy for better performance
         # NOTE: np.isin requires list (not set)
-        all_indices = np.arange(len(dataset), dtype=np.int32)
+        all_indices = np.arange(len(dataset), dtype=np.int64)
         classes = np.array([dataset.getitem_class(i) for i in all_indices])
         if self.valid_classes is not None:
             indices = all_indices[np.isin(classes, list(self.valid_classes))]
         else:
             indices = all_indices[~np.isin(classes, list(self.invalid_classes))]
         super().__init__(dataset=dataset, indices=indices)
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 import numpy as np
 import torch
 
 from kappadata.datasets.kd_subset import KDSubset
 from kappadata.utils.class_counts import get_class_counts
+from kappadata.utils.getall_class_as_tensor import getall_class_as_tensor
 
 
 class OversamplingWrapper(KDSubset):
     def __init__(self, dataset, strategy="multiply"):
         self.strategy = strategy
 
-        if hasattr(dataset, "getall_class"):
-            classes = dataset.getall_class()
-            if isinstance(classes, np.ndarray):
-                classes = torch.from_numpy(classes)
-            elif not torch.is_tensor(classes):
-                classes = torch.tensor(classes)
-        else:
-            classes = torch.tensor([dataset.getitem_class(i) for i in range(len(dataset))])
-        class_counts = get_class_counts(classes, dataset.getdim_class())
+        classes = getall_class_as_tensor(dataset)
+        class_counts, _ = get_class_counts(classes, dataset.getdim_class())
         max_class_count = torch.max(class_counts)
         indices = torch.arange(len(dataset), dtype=torch.long)
         if self.strategy == "multiply":
             # append miniority classes as long as they are not bigger than the majority class
             for i in range(len(class_counts)):
                 # if class is not contained in dataset -> cant multiply sample
                 if class_counts[i] == 0:
@@ -30,8 +24,8 @@
                 if multiply_factor > 0:
                     # get indices of samples with class to oversample
                     all_indices = torch.arange(len(dataset), dtype=torch.long)
                     sample_idxs = all_indices[classes == i]
                     indices = torch.concat([indices, torch.tile(sample_idxs, dims=[multiply_factor])])
         else:
             raise NotImplementedError(f"invalid oversampling strategy {self.strategy}")
-        super().__init__(dataset=dataset, indices=indices.tolist())
+        super().__init__(dataset=dataset, indices=indices)
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
         self.from_index = self.from_percent * len(dataset)
         self.from_index = np.ceil(self.from_index) if self.ceil_from_index else int(self.from_index)
 
         self.to_index = self.to_percent * len(dataset)
         self.to_index = np.ceil(self.to_index) if self.ceil_to_index else int(self.to_index)
 
-        indices = np.arange(self.from_index, self.to_index, dtype=np.int32)
+        indices = np.arange(self.from_index, self.to_index, dtype=np.int64)
         super().__init__(dataset=dataset, indices=indices)
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/repeat_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         if min_size is not None:
             assert isinstance(min_size, int) and min_size > 0
             self.repetitions = int(np.ceil(min_size / len(dataset)))
         else:
             assert repetitions > 0
 
         # repeat indices <repetitions> times in round-robin fashion (indices are like [0, 1, 2, 0, 1, 2])
-        indices = np.tile(np.arange(len(dataset), dtype=np.int32), self.repetitions)
+        indices = np.tile(np.arange(len(dataset), dtype=np.int64), self.repetitions)
         super().__init__(dataset=dataset, indices=indices)
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/dataset_wrappers/subset_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/dataset_wrappers/subset_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,25 @@
                 # create indices from start/end index
                 assert start_index is None or isinstance(start_index, int)
                 assert end_index is None or isinstance(end_index, int)
                 end_index = end_index or len(dataset)
                 end_index = min(end_index, len(dataset))
                 start_index = start_index or 0
                 assert start_index <= end_index
-                indices = np.arange(start_index, end_index, dtype=np.int32)
+                indices = np.arange(start_index, end_index, dtype=np.int64)
             elif start_percent is not None or end_percent is not None:
                 # create indices from start/end percent
                 assert start_percent is None or (isinstance(start_percent, (float, int)) and 0. <= start_percent <= 1.)
                 assert end_percent is None or (isinstance(end_percent, (float, int)) and 0. <= end_percent <= 1.)
                 start_percent = start_percent or 0.
                 end_percent = end_percent or 1.
                 assert start_percent <= end_percent
                 start_index = int(start_percent * len(dataset))
                 end_index = int(end_percent * len(dataset))
-                indices = np.arange(start_index, end_index, dtype=np.int32)
+                indices = np.arange(start_index, end_index, dtype=np.int64)
             else:
                 raise RuntimeError
         else:
             assert start_index is None and end_index is None
             assert start_percent is None and end_percent is None
             for i in indices:
                 assert -len(dataset) <= i < len(dataset)
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py` & `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,18 @@
         # initialize
         self.mixup_alpha = mixup_alpha
         self.cutmix_alpha = cutmix_alpha
         self.mixup_p = mixup_p
         self.cutmix_p = cutmix_p
         self.seed = seed
         # rng with seed is set in _shared
-        self.rng = np.random.default_rng()
+        # problem: if no seed is passed -> default_rng will not be affected by np.random.set_seed
+        # solution: sample a random integer from np.random.randint (which is affected by np.random.set_seed)
+        seed = np.random.randint(np.iinfo(np.int32).max)
+        self.rng = np.random.default_rng(seed=seed)
 
         # TODO port to per property key
         self.ctx_key = self.ctx_prefix
 
     @property
     def total_p(self) -> float:
         return self.mixup_p + self.cutmix_p
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 from dataclasses import dataclass
 
 import numpy as np
 
 from kappadata.datasets.kd_wrapper import KDWrapper
 from kappadata.factory import object_to_transform
 from kappadata.transforms import KDTransform, KDComposeTransform, KDStochasticTransform, KDIdentityTransform
+from .x_transform_wrapper import XTransformWrapper
 
 
 @dataclass
 class KDMultiViewConfig:
     n_views: int
     transform: callable
 
 
 class KDMultiViewWrapper(KDWrapper):
     def __init__(self, dataset, configs, seed=None):
         super().__init__(dataset=dataset)
+        # if dataset is XTransformWrapper -> check that transform is deterministic (can only check KDTransforms)
+        if isinstance(dataset, XTransformWrapper):
+            assert dataset.transform.is_deterministic
+
         assert isinstance(configs, list)
         # copy to not alter the original list
         configs = deepcopy(configs)
         # parse configs
         for i in range(len(configs)):
             if not isinstance(configs[i], KDMultiViewConfig):
                 if isinstance(configs[i], (list, tuple)):
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,35 @@
 
 from kappadata.datasets.kd_wrapper import KDWrapper
 
 
 class LabelSmoothingWrapper(KDWrapper):
     def __init__(self, dataset, smoothing):
         super().__init__(dataset=dataset)
-        assert isinstance(smoothing, (int, float)) and 0. < smoothing < 1.
+        assert isinstance(smoothing, (int, float)) and 0. <= smoothing <= 1.
         self.smoothing = smoothing
 
     def getitem_class(self, idx, ctx=None):
         y = self.dataset.getitem_class(idx, ctx)
+        if self.smoothing == 0:
+            return y
         assert isinstance(y, int) or (torch.is_tensor(y) and y.ndim == 0)
         n_classes = self.dataset.getdim_class()
+
+        # semi supervised case (can't smooth missing labels)
+        if y == -1:
+            return torch.full(size=(n_classes,), fill_value=-1.)
+
+        # binary case (label is scalar)
+        if n_classes == 1:
+            off_value = self.smoothing / 2
+            if y > 0.5:
+                return y - off_value
+            else:
+                return y + off_value
+
+        # multi class (scalar -> vector)
         off_value = self.smoothing / n_classes
         on_value = 1. - self.smoothing + off_value
         y_vector = torch.full(size=(n_classes,), fill_value=off_value)
         y_vector[y] = on_value
         return y_vector
```

### Comparing `kappadata-1.2.9/kappadata/wrappers/torch_wrapper.py` & `kappadata-1.3.0/kappadata/wrappers/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `kappadata-1.2.9/kappadata.egg-info/PKG-INFO` & `kappadata-1.3.0/kappadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kappadata
-Version: 1.2.9
+Version: 1.3.0
 Summary: pytorch dataset wrappers for in-memory caching
 Home-page: https://github.com/BenediktAlkin/KappaData
 Project-URL: Source Code, https://github.com/BenediktAlkin/KappaData
 Project-URL: Bug Tracker, https://github.com/BenediktAlkin/KappaData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 - various dataset filters and other dataset manipulation
     - filter by class
     - limit size to a %
     - [Mixup](https://arxiv.org/abs/1710.09412)
     - [Cutmix](https://arxiv.org/abs/1905.04899)
     - label smoothing
     - ...
+- repeated augmentations
 
 # Modular datasets
 
 [pytorch datasets](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) load all data in the `__getitem__`.
 KappaData decouples the `__getitem__` such that single properties of the dataset can be loaded independently.
 
 ## Image classification dataset example
```

### Comparing `kappadata-1.2.9/kappadata.egg-info/SOURCES.txt` & `kappadata-1.3.0/kappadata.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -28,59 +28,74 @@
 kappadata/common/datasets/kd_image_folder.py
 kappadata/common/transforms/__init__.py
 kappadata/common/transforms/byol_transforms.py
 kappadata/common/transforms/imagenet_minaug_transforms.py
 kappadata/common/transforms/imagenet_noaug_transforms.py
 kappadata/common/transforms/mae_finetune_transform.py
 kappadata/common/transforms/norm/__init__.py
+kappadata/common/transforms/norm/kd_ade20k_norm.py
 kappadata/common/transforms/norm/kd_cifar100_norm.py
 kappadata/common/transforms/norm/kd_cifar10_norm.py
 kappadata/common/transforms/norm/kd_image_net_norm.py
 kappadata/common/wrappers/__init__.py
 kappadata/common/wrappers/sample_wrappers/__init__.py
 kappadata/common/wrappers/sample_wrappers/byol_multi_view_wrapper.py
 kappadata/common/wrappers/sample_wrappers/imagenet_minaug_multi_view_wrapper.py
 kappadata/common/wrappers/sample_wrappers/imagenet_minaug_x_transform_wrapper.py
 kappadata/common/wrappers/sample_wrappers/imagenet_noaug_x_transform_wrapper.py
 kappadata/copying/__init__.py
+kappadata/copying/folder.py
 kappadata/copying/image_folder.py
 kappadata/datasets/__init__.py
 kappadata/datasets/kd_concat_dataset.py
 kappadata/datasets/kd_dataset.py
 kappadata/datasets/kd_subset.py
 kappadata/datasets/kd_wrapper.py
 kappadata/loading/__init__.py
 kappadata/loading/image_folder.py
 kappadata/samplers/__init__.py
+kappadata/samplers/distributed_sampler.py
 kappadata/samplers/infinite_batch_sampler.py
 kappadata/samplers/interleaved_sampler.py
+kappadata/samplers/random_sampler.py
+kappadata/samplers/semi_sampler.py
+kappadata/samplers/sequential_sampler.py
 kappadata/transforms/__init__.py
-kappadata/transforms/add_gaussian_noise_transform.py
 kappadata/transforms/image_pos_embed_grid.py
 kappadata/transforms/image_pos_embed_sincos.py
+kappadata/transforms/kd_additive_gaussian_noise.py
 kappadata/transforms/kd_bucketize.py
 kappadata/transforms/kd_color_jitter.py
+kappadata/transforms/kd_columnwise_norm.py
 kappadata/transforms/kd_gaussian_blur_pil.py
 kappadata/transforms/kd_gaussian_blur_tv.py
+kappadata/transforms/kd_grayscale.py
+kappadata/transforms/kd_horizontal_flip.py
+kappadata/transforms/kd_minsize.py
 kappadata/transforms/kd_rand_augment.py
 kappadata/transforms/kd_rand_augment_custom.py
+kappadata/transforms/kd_random_additive_gaussian_noise.py
 kappadata/transforms/kd_random_apply.py
 kappadata/transforms/kd_random_color_jitter.py
 kappadata/transforms/kd_random_crop.py
 kappadata/transforms/kd_random_erasing.py
 kappadata/transforms/kd_random_gaussian_blur_pil.py
 kappadata/transforms/kd_random_gaussian_blur_tv.py
 kappadata/transforms/kd_random_grayscale.py
 kappadata/transforms/kd_random_horizontal_flip.py
 kappadata/transforms/kd_random_resized_crop.py
 kappadata/transforms/kd_random_rotation.py
 kappadata/transforms/kd_random_solarize.py
+kappadata/transforms/kd_random_threshold.py
 kappadata/transforms/kd_rearrange.py
 kappadata/transforms/kd_resize.py
+kappadata/transforms/kd_simple_random_crop.py
 kappadata/transforms/kd_solarize.py
+kappadata/transforms/kd_three_augment.py
+kappadata/transforms/kd_threshold.py
 kappadata/transforms/kd_two_random_crop.py
 kappadata/transforms/patchify_image.py
 kappadata/transforms/patchwise_norm.py
 kappadata/transforms/patchwise_random_rotation.py
 kappadata/transforms/patchwise_shuffle.py
 kappadata/transforms/save_state_to_context_transform.py
 kappadata/transforms/unpatchify_image.py
@@ -90,45 +105,63 @@
 kappadata/transforms/base/kd_random_apply_base.py
 kappadata/transforms/base/kd_scheduled_transform.py
 kappadata/transforms/base/kd_stochastic_transform.py
 kappadata/transforms/base/kd_transform.py
 kappadata/transforms/norm/__init__.py
 kappadata/transforms/norm/kd_image_norm.py
 kappadata/transforms/norm/kd_image_range_norm.py
-kappadata/transforms/norm/base/__init__.py
-kappadata/transforms/norm/base/kd_norm_base.py
+kappadata/transforms/norm/kd_norm_base.py
+kappadata/transforms/semseg/__init__.py
+kappadata/transforms/semseg/kd_semseg_pad.py
+kappadata/transforms/semseg/kd_semseg_random_crop.py
+kappadata/transforms/semseg/kd_semseg_random_horizontal_flip.py
+kappadata/transforms/semseg/kd_semseg_random_resize.py
+kappadata/transforms/semseg/kd_semseg_resize.py
 kappadata/utils/__init__.py
 kappadata/utils/bounding_box_utils.py
 kappadata/utils/class_counts.py
 kappadata/utils/color_histogram.py
+kappadata/utils/distributed.py
+kappadata/utils/getall_class_as_tensor.py
+kappadata/utils/hash_utils.py
+kappadata/utils/image_utils.py
 kappadata/utils/logging.py
 kappadata/utils/magnitude_sampler.py
 kappadata/utils/multi_crop_utils.py
 kappadata/utils/one_hot.py
 kappadata/utils/param_checking.py
 kappadata/utils/pos_embed.py
 kappadata/utils/save_image.py
 kappadata/utils/transform_utils.py
 kappadata/visualization/__init__.py
+kappadata/visualization/visualize_dataset_imgsize.py
+kappadata/visualization/visualize_interpolation.py
+kappadata/visualization/visualize_jigsaw.py
+kappadata/visualization/visualize_mae_schematic.py
+kappadata/visualization/visualize_masked_image.py
+kappadata/visualization/visualize_transform.py
 kappadata/visualization/visualize_two_random_crop.py
 kappadata/wrappers/__init__.py
 kappadata/wrappers/mode_wrapper.py
 kappadata/wrappers/torch_wrapper.py
 kappadata/wrappers/dataset_wrappers/__init__.py
 kappadata/wrappers/dataset_wrappers/class_filter_wrapper.py
 kappadata/wrappers/dataset_wrappers/classwise_subset_wrapper.py
 kappadata/wrappers/dataset_wrappers/oversampling_wrapper.py
+kappadata/wrappers/dataset_wrappers/overwrite_classes_wrapper.py
 kappadata/wrappers/dataset_wrappers/percent_filter_wrapper.py
 kappadata/wrappers/dataset_wrappers/repeat_wrapper.py
 kappadata/wrappers/dataset_wrappers/shuffle_wrapper.py
 kappadata/wrappers/dataset_wrappers/subset_wrapper.py
 kappadata/wrappers/sample_wrappers/__init__.py
 kappadata/wrappers/sample_wrappers/kd_mix_wrapper.py
 kappadata/wrappers/sample_wrappers/kd_multi_view_wrapper.py
 kappadata/wrappers/sample_wrappers/label_smoothing_wrapper.py
 kappadata/wrappers/sample_wrappers/one_hot_wrapper.py
+kappadata/wrappers/sample_wrappers/semseg_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/source_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/target_transform_wrapper.py
+kappadata/wrappers/sample_wrappers/x_repeat_wrapper.py
 kappadata/wrappers/sample_wrappers/x_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/y_transform_wrapper.py
 kappadata/wrappers/sample_wrappers/base/__init__.py
 kappadata/wrappers/sample_wrappers/base/transform_wrapper_base.py
```

### Comparing `kappadata-1.2.9/setup.cfg` & `kappadata-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.9
+version = 1.3.0
 name = kappadata
 description = pytorch dataset wrappers for in-memory caching
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BenediktAlkin/KappaData
 project_urls = 
 	Source Code = https://github.com/BenediktAlkin/KappaData
```

